# TomoFlex2
---
TomoFlex is a flexible travel-time tomography package capable of joint inversion with various data types (e.g. absolute and differential P/S arrival times, S-P times), and functional with source location separately or simultaneously, a priori model correction (e.g. near-surface logging data).
---

PACKAGE LAYOUT:
        src           -- Backup of source codes
        example       -- A work zone for inversion, containing the directory
                         "DEMO" for start
        utils         -- Some plotting scripts compiled here for displaying
                         the results
        doc           -- Package-related references


S.O.P OF INVERSION:
        1) Into directory "example". Start by copying the "DEMO" to another
           one with any desired name related to your study (say TEST)
        2) In "TEST", there is one subdirectory called "inv". Replace the
           input data (station, event, travel times, and velocity model) by
           yours and modify the parameters in the control file "tomo.inp"
        3) Simply type "make" for running the inversion! Note that for the
           first time running in "inv", it is strongly suggested to type
           "make clean" before typing "make"
        4) Then pretty much every thing is done. Waiting for your results
           and playing with the parameters for testing and verifying

        Two other subdirectories "make3dmod" and "fwd" in "TEST" are for makeing
        the 3D velocity model from the 1D one and for computing the synthetic
        travle times, respectively. Details of usage please refer to the
        "README" in "DEMO"

        
