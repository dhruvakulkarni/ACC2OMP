# ACC2OMP

# Description
A Python script to facilitate source-to-source translation from OpenACC to OpenMP.

This tool was written to lower the barrier for Fortran software projects that have been using the OpenACC programming model
and want to migrate to the OpenMP 4.5 programming model. For the most part, there is a 1-to-1 mapping between OpenACC directives
and OpenMP directives with some exceptions.

Please note that is very much a work-in-progress (WIP) and has several known limitations documented below:

# Known limitations
- OpenACC -> OpenMP directive mapping must be explicitly available in a dictionary
- OpenACC async is not handled properly because of fundamental differences between OpenACC and OpenMP
- Only handles Fortran
- Search string tokens are case dependent
- Lack of proper handling of line indentation
- No unit tests
- No enforcement of PEP8 formating on source code

# Funding
This research was supported by the Exascale Computing Project (17-SC-20-SC), a joint project of the U.S. Department of Energy’s
Office of Science and National Nuclear Security Administration, responsible for delivering a capable exascale ecosystem, including
software, applications, and hardware technology, to support the nation’s exascale computing imperative.
