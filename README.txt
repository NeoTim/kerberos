
              Kerberos PA-REQ examples
              ------------------------

* About

  In November 2008 on the InsidePro forums, a poster requested code for
  some implementation of how kerberos authentication for windows
  worked. [1]

  I provided some basic code on how to verify password using information
  from RFC4757 describing the algorithm in detail. [2]

  Since then, a module (mskrb5) by magnum was implemented for John The
  Ripper based on code krb_rc4.cpp [3]

  Later in March 2009, I decided to look at how it worked for Vista since it
  was no longer using RC4/HMAC-MD5 for authentication against Windows 2008
  domain controllers.

  Using RFC3961 [4] and RFC3962 [5] another example was provided (krb_aes.cpp)
  which led to another JtR module by Dhiru [6]


* References

[1] Kerberos Pre-authentication
    http://forum.insidepro.com/viewtopic.php?t=2396&highlight=

[2] The RC4-HMAC Kerberos Encryption Types Used by Microsoft Windows
    http://tools.ietf.org/rfc/rfc4757.txt

[3] MS Kerberos 5 "PA ENC TIMESTAMP" by magnum
    https://github.com/magnumripper/JohnTheRipper/blob/unstable-jumbo/src/krb5pa-md5_fmt_plug.c

[4] Encryption and Checksum Specifications for Kerberos 5
    http://www.ietf.org/rfc/rfc3961.txt

[5] Advanced Encryption Standard (AES) Encryption for Kerberos 5
    http://tools.ietf.org/rfc/rfc3962.txt

[6] Kerberos 5 "PA ENC TIMESTAMP" by magnum (modified by Dhiru)
    https://github.com/magnumripper/JohnTheRipper/blob/unstable-jumbo/src/krb5pa-sha1_fmt_plug.c
