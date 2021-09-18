### Fortran FAQ

 Here are some answers to frequently asked questions. The "author", as is
 the custom, has appropriated posted responses as seemed apt. I have tried
 to leave attributions in, as correctly as possible. To anyone who has been
 offended by omission or otherwise, my apologies. I shall give priority to
 corrections regarding attribution.

 No one takes responsibility for any of this text, neither the employer of
 the "author", the "author", friends of the "author", pets of the "author"
 nor anyone else.

 Your mileage WILL vary.

 A good place to look for FAQ's is:

    host:       rtfm.mit.edu
    directory:  /pub/usenet

 The structure of the current list has been modified from previous versions
 in an attempt to group related questions according to their topic, and to
 maintain consistency with the new order.  Let the author know if any
 inconsistencies have been introduced by the revision. <William B. Clodius
 contributed the reorganization> A more recent reorganization, and htmlization
 (which is what this ascii text is derived from) thanks to Abraham Agay.

     ,;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;,
     ;;                                       ;;
     ;;    Numbering convention:              ;;
     ;;    '''''''''''''''''''''              ;;
     ;;    l)         General Category:       ;;
     ;;      l.m)     Topic:                  ;;
     ;;        l.m.n) Question:               ;;
     ;;                                       ;;
     `;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;'


    SUMMARY OF CHANGES
    ==================

C      1.2.4   Added
C      2.      Updated
C      +  misc other updates (bad bookkeeping)

       1.2.1   Updated

  ;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;



1) GENERAL INTEREST:


  1.1) The language and its development


    1.1.0) How should one spell FORTRAN/Fortran? 

    1.1.1) Where can I learn more about the history of Fortran? 

    1.1.2) How does Fortran 90 relate to FORTRAN '77 and what is Fortran 90? 

    1.1.3) Is Fortran 90 a Standard? Where can I get a copy of the Fortran 90
           Standard? How about electronic copies? (getting other standards) 

    1.1.4) Who creates these silly standards anyway? 

    See also:

           2.1.5) Tell me about Parallel Fortran dialects, what are they, etc. 


  1.2) Learning Fortran and its style


    1.2.1) What are good books on Fortran? 

    1.2.2) Where can I find a f90 tutorial or course? 

    1.2.3) What constitutes good FORTRAN style? 

    1.2.4) What is a good subset of Fortran? 


  1.3) General Fortran (particularly Fortran 90) resources


    1.3.1) f90.faq from Michel Olagnon 

    1.3.2) f90 "market" announcement from walt brainerd 


2) TOOLS:


  2.1) Compilers


    2.1.1) Where can I get a free (FORTRAN 77) compiler? 

    2.1.2) What is the best (FORTRAN 77) compiler for a PC? 

    2.1.3) What is the best Fortran for... 

    2.1.4) What Fortran 90/95 compilers/translators are available? 

    2.1.5) Tell me about Parallel Fortran dialects, what are they, etc. 

    See also:

           2.2.6) What is preprocessing, how can it help? How can it hurt? 

           3.1.4) For whatever reasons, I want to translate my Fortran into C.
                  What tools are available? 


  2.2) Other tools (pretty printers, lints, converters, etc.)


    2.2.1) I have heard of fortran "lints"; what are they, and where can
           I get one? 

    2.2.2) Are there pretty printers for FORTRAN? Flowchart generators? 

    2.2.3) Is there a WEB for Fortran (and what is WEB anyway)? 

    2.2.4) Fortran text editors? 

    2.2.5) How can I convert an existing FORTRAN 77 program
           to the free form source of Fortran 90? 

    2.2.6) What is preprocessing, how can it help? How can it hurt? 


  2.3) Fortran Packages and libraries


    2.3.1) Where can I get "foo" (some random package), older posts
       to comp.lang.fortran etc  

    2.3.2) Where can I find coded BLAS (and what are coded BLAS?) 

    2.3.3) Where can I get mathematical software? 

    2.3.4) What Interval Arithmetic packages are avaliable? 

    2.3.5) FLIB announcement 


3)  TECHNICAL QUESTIONS:


  3.1) Fortran and other languages (essentially C)


    3.1.1) "Why do people use FORTRAN? C is so much better" 

    3.1.2) Why are there aimless debates? 

    3.1.3) How do I call f77 from C (and visa versa) 

    3.1.4) For whatever reasons, I want to translate my Fortran into
           C. What tools are available? 

    3.1.5) For whatever reasons, I want to translate my existing C code
           into Fortran. What tools are available? 


  3.2) System differences


    3.2.1) My compiler is mis-behaving; who enforces the standard? 

    3.2.2) My F77 program compiled ok on a <system1>, but gives me heaps
           of syntax errors on a <system2>. What's wrong? 

    3.2.3) My F77 program ran ok on a <system1>, but on a <system2>
           it just gives me strange results. What's wrong? 

    3.2.4) How can I read my VAX binary data somewhere else? 


  3.3) Language extensions


    3.3.1) How common is DO ... END DO? 

    3.3.2) What are ENCODE and DECODE statements, and how are they translated
           to standard Fortran? How can I convert numbers to character strings
           (and vice-versa)? 


  3.4) .......


    3.4.1) What is involved in parsing Fortran? 


4)  WWW SOFTWARE/FORTRAN


   4.1.1) WWW and Fortran 


 Start of contents 


  ;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;


1.1) The language(s) and its(their) development


1.1.0) How should one spell FORTRAN/Fortran?

       FORTRAN is generally the preferred spelling for discussions
       of versions of the language prior to the current one ("90").
       Fortran is the spelling chosen by X3J3 and WG5.
       In this document a feeble effort has been made to capitalize
       accordingly (e.g. vast existing software ... FORTRAN vs.
       generic Fortran to mean all versions of the standard,
       and specifically the modern dialect, ISO 1539:1991).


       ---------------------------------------
       ~From: walt@fortran.com (Walt Brainerd)
       ---------------------------------------

       There was an effort to "standardize" on spelling of programming
       languages just after F77 became a standard.  The rule: if you say
       the letters, it is all caps (APL); if you pronounce it as a word,
       it is not (Cobol, Fortran, Ada).  See, for example the definitive
       article describing Fortran 77 in the Oct 1978 issue of the Comm.
       of the ACM.  The timing was such that FORTRAN got put on the
       standard itself, though many always after that have referred to
       it as Fortran 77.  Of course, there are those who think it is
       not truly Fortran if not written with all caps.

<ed note>

       ISO 1539:1991 and its ANSI counterpart X3.198-1992 consistently
       employ the spelling "Fortran" to refer to the language being
       defined. Reference(s) to the older version employ "small caps"
       for the "ORTRAN" characters.


   __________________________________________________________________________
                                       


1.1.1) Where can I learn more about the history of Fortran?
 
       The book "Abstracting Away the Machine: The History of the FORTRAN Programming Language (FORmula TRANslation)"
       was self-published by Mark Jones Lorenzo in 2019 https://www.amazon.com/Abstracting-Away-Machine-Programming-TRANslation/dp/1082395943 
       and has been favorably received. Also see the Fortran Wiki http://fortranwiki.org/fortran/show/Fortran+History and Wikipedia.

       -------------------------------------------------
       ~From: metcalf@apofort.cern.ch (Michael Metcalf )
       -------------------------------------------------

       The history of Fortran is documented in:

       Annals of History of Computing,
          6, 1, January, 1984 (whole issue)

       Programming Systems and Languages
          (S. Rosen ed.),
          McGraw Hill, 1967,
          pp 29-47 (this is Backus's original paper)

       History of Prorammining Languages
          (R.L. Wexelblat ed.),
          Academic Press, 1981,
          pp 25-74


       A summary appears in:

          Encyclopedia of Science and Technology,
             Academic Press, 1986,
             vol. 5, under 'Fortran'

       and in:

          Fortran 90 Explained
             (Oxford, 1990).
             Chapter 1 of


   __________________________________________________________________________
                                       


1.1.2) How does Fortran 90 relate to FORTRAN '77?

       With a few minor exceptions, Fortran 90 is a superset of
       X3.9-1978 FORTRAN.

       But this does not mean that all "77" codes will port sans changes.
       Many (if not most) programmers employed constructs beyond the '77
       standard, or rely on unspecified behavior (say, assuming that an
       OPEN of an existing file will position the file pointer to just
       past the last record already written) which has changed (that is
       to say, has become specified).

       This leads to the obvious question, what is new in Fortran 90?

       A complete answer would require considerable text.
       Some of the most obvious additions are:

          1) array notation (operators, etc.)
          2) dynamic memory allocation
          3) derived types and operator overloading
          4) keyword argument passing, INTENT (in, out, inout)
          5) modules
          6) modern control structures
          7) free format source code form
          8) other stuff

       While it is always tricky to characterize the motives of
       a large group of people, I <khb> am inclined to try
       as follows:

       '90 incorporates two sets of improvements:

          (1) relatively minor fixups that *could* have been
              done earlier

          (2) relatively major changes to enable better software
              engineering practices.

       Sometimes a "minor" fixup has major effect, such as addition
       of free form source form combined with canonization of the
       MIL-STD 1753 INCLUDE.

       I further go off on a limb and assert that it was the goal
       of the *committee* to evolve Fortran in a fashion to enable
       it to continue to be the premier language for scientific
       computation.


   __________________________________________________________________________
                                       


1.1.3) Is it a Standard? Where can I get a copy of the Fortran 90
       Standard? How about electronic copies?

       Fortran 90 was adopted as an International Standard by ISO
       in July, 1991.  It was published by them as ISO/IEC 1539:1991,
       and is obtainable directly for 185 Swiss francs from:

           ISO Publications
              1 rue de Varembe
              Case postale 56
              CH-1211 Geneva 20
              Switzerland
              Fax:  + 41 22 734 10 79

       or from:

           American National Standards Institute
              Attn: Customer Service
              11 West 42nd Street
              New York, NY 10036
              Phone: (212)642-4900 8:45-4:45 (EST)
              Fax:   (212)302-1286

           BSI
              2 Park Street
              London W1A 2BS

           DIN
              Burggrafenstrasse 6
              Postfach 1107
              D-1000 Berlin 30

           AFNOR
              Tour Europe
              Cedex 7
              92049 Paris La Defence

           SCC
              1200-45 O'Connor
              Ottawa
              Ontario  K1P 6N7


       You can obtain copies for $225 through:

           Global Engineering Documents
              2805 McGaw Ave.
              Irvine, CA. 92714
              (714) 261-1455
              (800) 854-7179


       In accordance with an official agreement with the International
       Standards Organization, Unicomp is now able to distribute
       electronic versions of the Fortran 90 standard:

          ISO/IEC 1539 : 1991,
          Information technology--Programming languages--Fortran

       The money received from this effort will go partly to fund ISO
       activities and partly to recover the costs incurred by Unicomp
       in preparing and typesetting the standard document.
       The prices are set by ISO.

       The document can be obtained in three versions:

          1. An ASCII version suitable for viewing on a computer
             terminal using any kind of editor.  Cost: USD 125.

          2. A PostScript version with a license allowing the
             purchaser to print n paper copies.  Cost: USD 125 + 10n.

          3. Complete source in ditroff with macros and software to
             extract and create the annexes.  The source constitutes
             a fairly high level marked-up document; for example,
             each program beginning and ending is marked and there
             are few low-level typographic commands such as size
             and font changes.  Cost USD 1000.

       I am quite enthused especially about version (2).  If you want
       to have 10 copies for your organization, and it costs $10 to
       make a printed copy, then the cost to make the 10 copies would
       be $125 + $200, or just $32.50 per copy, which is a substantial
       savings over purchasing paper copies.

       Versions (1) and (3) will be accompanied by a license restricting
       use to one CPU and prohibiting copying, except for backup purposes,
       etc. The version (2) license will prohibit distributing any of the
       printed copies outside of the purchasing organization.

       If you have special requirements, such as wanting to distribute
       a copy with each version of your compiler or using the source
       as a part of your documentation, we can make special arrangements,
       subject to the approval of the ISO.  Please advise me of your
       requirements and we can work up a proposal together.

       ISO and Unicomp think this will provide the oft requested access
       to the standard in electronic form. This is the first time this
       is being tried, so we hope that organizations will be careful to
       observe the rules and encourage the continued availability of
       this and other standards in electronic form.

       Payment can be made by Visa or MasterCard, or with a check on
       a US Bank in US funds.  We <unicomp> will accept a purchase
       order only if the amount is $500 or more.

          Walter S. Brainerd; Unicomp;
          phone:  505-275-0800.
          email:  Walt Brainerd <walt@fortran.com>


;;; Additional note.

       X3J3 working papers are often available via
       ftp from:

          host:       ftp.ncsa.uiuc.edu
          directory:  x3j3

rpc wrote:

       It has been a few years since I last ordered a MIL-STD, so my
       information might be out-of-date.  At that time, the address
       to write for MIL-STDs was:

          Naval Publications and Forms Center, Code 3015
          5801 Tabor Ave
          Philadelphia, PA 19120

          Phone:  1-(215)-697-4834

       Use form DD1425, if possible (they will send you a copy with
       your first order).

       MIL-STD 1753 is a short document (about 10 pages).

       And finally, note that the FORTRAN 77 standard is online at
       the Fortran Market:

          http://www.fortran.com/fortran/market.html
          http://www.fortran.com/walt/fortran



   __________________________________________________________________________
                                       


1.1.4) Who creates these silly standards anyway?

       Typically X3J3. X3J3 is an ANSI subcommittee dedicated to Fortran.
       WG5 is the ISO counterpart. WG5 owns responsibility for Fortran
       on an international basis. WG5 has previously tasked X3J3 to do
       the work. This arrangement continues.

       WG5 is composed of Fortran users, vendors, and academics
       from several ISO supporting nations. Delegates represent
       *their*countries* not their companies; so several delegates
       from a single company is permitted.

       ANSI rules prohibit multiple voting delegates from the same company.
       X3J3 is composed of users (aerospace, government labs, military,
       DECUS, railroads, oil to name a few), vendors (IBM, CRI, Sun,
       Convex, DEC, UNISYS, to name a few) and the odd academic
       (oxford, yale, liverpool, to name a couple).
       Members need not be US citizens nor must their company be US
       domiciled.  Being a member of a standards group is typically
       involves non-trivial work.
       To be effective, one should plan on at least 8 weeks of time
       per year (those who are really doing the hard work do far more).
       This time commitment is typically far more expensive than the
       travel and membership costs.

       X3J3 meetings are open to the public. There are typically 4
       meetings a year, typically 3 are in the US and 1 *may* be
       overseas (to precede or follow the WG5 plenary session).
       Membership fees are levied by ANSI, and are on the near order
       of $600 ($300ish cast as an ISO "tax", but mandatory for all).
       In addition, attendees to a particular X3J3 meeting pay a
       "meeting fee" which covers reproduction costs, snacks and etc.
       The meeting fee has been about $100 for the last several meetings.

       WG5 has established various goals and targets for future work.
       Roughly speaking 5yrs rather than 13years are the targets for
       future work.

       Current work projects include cleanup and interpretations
       of Fortran (90), features for future versions of the standard
       (e.g.  parallel processing, "object-oriented" technologies, etc.).
       In addition to work done directly by X3J3, there is work on
       standardized modules, and OS bindings taking place in other
       organizations. X3J3 would like to keep track of such efforts,
       those involved are invited to inform X3J3 early in their
       development efforts if possible. X3J3 is currently working
       with X3H5, DIN (varying string character) and tracking the
       efforts of HPFF.

       New members are always welcome. Visitors are also; though it
       is very hard to get a good grip on things in only one meeting!

       Contact the X3J3 chair for more information:

          email:  jwagener@trc.amoco.com      (chair)

       Upcoming meeting is:  5 Feb - 9 Feb   Las Vegas

       papers are often available via ftp from:

          host:       ftp.ncsa.uiuc.edu
          directory:  x3j3


   __________________________________________________________________________
                                       


B) Learning Fortran


1.2.1) What are good books on Fortran?

       Don't know if they are good. Inclusion in the list
       is not endorsement.

On Fortran 90:

   English:

       Fortran 90
          Counihan,
          Pitman, 1991,
          ISBN 0-273-03073-6.

       Fortran 90 Explained
          Metcalf and Reid,
          Oxford University Press, 1990,
          ISBN 0-19-853772-7,
          about $30.

          This book is a complete, audited description of the language
          in a more readable style than the standard itself.
          It is kept up-to-date on each printing with X3J3 and WG5's
          latest interpretations.
          It has seven Appendices, including an extended example program
          that is available by ftp, and a comprehensive Index.

       Fortran 90/95 Explained
          Michael Metcalf and John Reid,
          Oxford University Press, Oxford and New York, 1996,
          ISBN 0 19 851888 9
          (about $US33 or 16.95 pounds sterling).

          Sequel to 90 explained.

       Fortran 90 for Scientists and Engineers
          Brian D.  Hahn, Edward Arnold, 1994,
          ISBN 0-340-60034-9.

       Fortran 90 Handbook
          Adams, Brainerd, Martin, Smith and Wagener,
          McGraw-Hill, 1992,
          ISBN 0-07-000406-4.

       Fortran 90 Language Guide
          Gehrke,
          Springer, London, 1995,
          ISBN 3-540-19926-8

       Fortran 95 Language Guide
          Gehrke,
          Springer, London, 1996,
          ISBN 3-540-76062-8

       Fortran-90-Nachschlagewerk
          Gehrke,
          RRZN, 1993

       Fortran 90 Programming
          Ellis, Philips, Lahey,
          Addison Wesley, Wokingham, 1994,
          ISBN 0-201-54446-6.

       Migrating to Fortran 90
          James F.  Kerrigan,
          O'Reilly Associates,
          1993, ISBN 1-56592-049-X.

       Programmer's Guide to Fortran 90, second edition
          Brainerd, Goldberg and Adams,
          Unicomp, 1994.

       Programming in Fortran 90
          Morgan and Schonfelder,
          Alfred Waller, Oxfordshire, 1993,
          ISBN 1-872474-06-3.

       Programming in Fortran 90
          I.M. Smith,
          Wiley,
          ISBN 0471-94185-9.

       Fortran 90,
          Loren P.  Meissner (U. of San Francisco) (c) 1995,
          PWS Publishing Co.,
          ISBN 0-534-93372-6

       Fortran 90:  A Reference Guide
          Luc Chamberland,
          Prentice-Hall, 1995,
          ISBN 0-13-397332-8

       Introducing Fortran 90
          Ian Chivers and Jane Sleightholme
          Springer Verlag,
          ISBN 3-540-19940-3

   Chinese:

       Programming Language FORTRAN 90
          He Xingui, Xu zuyuan, Wu gingbao and Chen mingyuan,
          China Railway Publishing House, Beijing,
          ISBN 7-113-01788-6/TP.187, 1994.

   Dutch:

       Fortran 90
          W.S.  Brainerd, Ch.H. Goldberg, and J.C. Adams,
          translated by J.M. den Haan,
          Academic Service, 1991,
          ISBN 90 6233 722 8.

   French:

       Fortran 90; Approche par la Pratique
          Lignelet,
          Se'rie Informatique E'ditions, Menton, 1993,
          ISBN 2-090615-01-4.

       Fortran 90.  Les concepts fondamentaux,
          the translation of "Fortran 90 Explained" M. Metcalf, J.  Reid,
          translated by M. Caillet and B. Pichon,
          AFNOR, Paris,
          ISBN 2-12-486513-7.

       Fortran 90; Initiation a` partir du Fortran 77
          Aberti,
          Se'rie Informatique E'ditions, Menton, 1992,
          ISBN 2-090615-00-6.

       Les specificites du Fortran 90,
          DUBESSET, M. et VIGNES, J.,
          editions Technip, 1993.
          ISBN 2-7108-0652-5

       Manuel complet du langage Fortran 90, et guide d'application,
          LIGNELET, P.,
          S.I. editions, Jan. 1995.
          ISBN 2-909615-02-2

       Programmer en Fortran 90,
          DELANNOY, C.,
          Eyrolles, 1992.
          ISBN 2-212-08723-3

       Savez-vous parler Fortran,
          AIN, M.,
          Bibliotheque des universites (de Boeck), 1994.
          ISBN 2-8041-1755-3

       Support de cours Fortran 90 IDRIS
          Corde, P. & Delouis, H.
          anonymous ftp from:

             host:       ftp.ifremer.fr
             directory:  pub/ifremer/fortran90/
             file:       f90_cours_4.ps.gz

       Traitement de donnees numeriques avec Fortran 90,
          Olagnon, M.
          Masson, 1996.
          ISBN 2-225-85259-6

          was just published this week. Though it is in French,
          the example programs

             http://www.ifremer.fr/ditigo/molagnon/livref90.html

          are in Fortran 90. One of them, CVIBM, deals with
          conversions between IEEE and former IBM format,
          and may be of some use to you.
          Anonymous ftp from:

             host:       ftp.ifremer.fr
             directory:  pub/ifremer/ditigo/fortran90/livremo/
             file:       cvibfl.f90


   German:


       Fortran 90
          B.Wojcieszynski and R.Wojcieszynski,
          Addison-Wesley, 1993,
          ISBN 3-89319-600-5.

       Fortran 90: eine informelle Einf"hrung
          Heisterkamp,
          BI-Wissenschaftsverlag, 1991,
          ISBN 3-411153-21-0.

       Fortran 90, Lehr- und Arbeitsbuch fuer das erfolgreiche Programmieren
          W.S.  Brainerd, C.H. Goldberg, and J.C. Adams,
          translated by Peter Thomas and Klaus G. Paul,
          R. Olbenbourg Verlag, Muenchen, 1994,
          ISBN 3-486-22102-7.

       Fortran 90 Lehr- und Handbuch
          T. Michel,
          BI-Wissenschaftsverlag, 1994.

       Fortran 90 Referenz-Handbuch: der neue Fortran-Standard
          Gehrke,
          Carl Hansen Verlag, 1991,
          ISBN 3-446163-21-2.

       Programmierung in Fortran 90
          Schobert,
          Oldenburg, 1991.

       Software Entwicklung in Fortran 90
          U"berhuber and Meditz,
          Springer Verlag, 1993,
          ISBN 0-387-82450-2.

   Japanese:

       Fortran 90 Explained
          Metcalf and Reid,
          translated by H. Nisimura, H. Wada, K.  Nishimura, M. Takata,
          Kyoritsu Shuppan Co., Ltd., 1993,
          ISSN 0385-6984.


On Fortran in general:

       Author                         Title                               Year
       ------                 -----------------------------               ----
       Kruger                 Efficient Fortran Programming               1990
       Mojena/Ageloff         FORTRAN 77                                  1990
       Boyle                  FORTRAN 77 PDQ                              1989
       Bezner                 FORTRAN 77                                  1989
       Tremblay               PROGRAMMING IN FORTRAN 77                   1988
       Salmon                 ENGINEERS & SCIENTISTS WITH FORTRAN 77      1988
       Nyhoff/Leestma         FORTRAN 77 FOR ENGINEERS & SCIENTISTS       1988
       McCracken/Salmon       ENGINEERS & SCIENTISTS WITH FORTRAN 77      1988
       Davis/Hoffman          FORTRAN 77: A STRUCTURED DISCIPLINED STYLE  1988
       Barnard/Skillicorn     FORTRAN 77 FOR ENGINEERS AND SCIENTISTS     1988
       Gregory A. Moses       Engineering Applications Software Develop.. 1988
       Gehrke                 PC-FORTRAN-Handbuch                         1988
       Mashaw                 PROGRAMMING STRUCTURED FORTRAN 77           1987
       Cole                   FORTRAN 77: A STRUCTURED ... APPROACH       1987
       Boillot                UNDERSTANDING FORTRAN-77                    1987
       Gehrke                 FORTRAN-77-Handbuch                         1987
       Starkey/Ross           FUNDAMENTAL PROGRAMMING WITH FORTRAN 77     1986
       Rouse/Bugnitz          INTRODUCTION TO FORTRAN 77                  1986
       Ratzer                 FORTRAN 77 COURSE                           1986
       Page                   FORTRAN 77 FOR HUMANS                       1986
       Lehman                 SOCIAL SCIENCES: ALGORITHMS & FORTRAN 77    1986
       Smith                  FORTRAN 77: A PROBLEM-SOLVING APPROACH      1985
       Shelly                 FORTRAN 77: AN INTRODUCTION                 1985
       Nickerson              FUNDAMENTALS OF FORTRAN 77 PROGRAMMING      1985
       Metcalf                EFFECTIVE FORTRAN 77                        1985
       Metcalf                FORTRAN Optimization                        1985
       McKeown                STRUCTURED PROGRAMMING USING FORTRAN 77     1985
       Hume                   FORTRAN 77 FOR SCIENTISTS & ENGINEERS       1985
       Dillman                PROBLEM SOLVING WITH FORTRAN 77             1985
       Brainerd               FORTRAN 77 FUNDAMENTALS AND STYLE           1985
       Borse                  FORTRAN 77&NUMERICAL METHODS FOR ENGINEERS  1985
       Adman                  FORTRAN 77 SOLUTIONS NON-SCIENTIFIC PROBS.  1985
       Etter                  PROBLEM SOLVING WITH STRUCTURED FORTRAN 77  1984
       Etter                  PROBLEM SOLVING USING FORTRAN 77             ?
       Dyck                   FORTRAN 77: A STRUCTURED APPROACH ...       1984
       Chivers/Clark          FORTRAN 77: A HANDS ON APPROACH             1984
       Adman                  FORTRAN 77 FOR NON-SCIENTISTS               1984
       Willamson/Levesque     A GUIDEBOOK TO FORTRAN ON SUPERCOMPUTER     1989
       Rule                   FORTRAN 77: A PRACTICAL APPROACH            1983
       Rouse/Bugnitz          PROGRAMMING THE IBM PC: FORTRAN 77          1983
       Nyhoff/Leestma         PROBLEM SOLVING WITH FORTRAN 77             1983
       Marateck               FORTRAN 77                                  1983
       Lehmnkuhl              FORTRAN 77                                  1983
       Law                    ANSI FORTRAN 77: INTRO. TO SOFTWARE DESIGN  1983
       Holoien/Behforooz      ... STRUCTURED PROGRAMMING WITH FORTRAN 77  1983
       Grout                  FUNDAMENTAL..PROGRAMMING USING FORTRAN 77   1983
       Fleming/Redish         THE U. S. MC MASTER GLOSSARY OF FORTRAN-77  1983
       Cole                   ANSI FORTRAN IV WITH FORTRAN 77 EXTENSIONS  1983
       Wu                     ANSI FORTRAN IV & 77 AND BUSINESS PROGRAMS  1982
       Pollack                STRUCTURED FORTRAN 77 PROGRAMMING           1982
       Katzan                 FORTRAN 77                                  1982
       Gibson/Young           INTRO TO PROGRAMMING USING FORTRAN 77       1982
       Ellis                  STRUCTURED APPROACH FORTRAN 77 PROGRAMMING  1982
       Durgin                 FORTRAN 77                                  1982
       Nanney                 A PROBLEM-SOLVING APPROACH USING FORTRAN77  1981
       Merchant               FORTRAN 77: LANGUAGE AND STYLE              1981
       Khailany               BUSINESS PROGRAMMING FORTRAN IV/ANSI F..    1981
       Ashcroft               PROGRAMMING WITH FORTRAN 77                 1981
       Gehrke                 FORTRAN-77-Sprachumfang                     1981
       Wagener                FORTRAN 77                                   ?
       Wagener                PRINCIPLES OF FORTRAN 77 PROGRAMMING        1980
       Meissner/Organick      FORTRAN77 FEATURING STRUCTURED PROGRAMMING  1980
       Hume/Holt              PROGRAMMING FORTRAN 77                      1979
       Balfour                PROGRAMMING IN STANDARD FORTRAN 77          1979


       A free Fortran 77 book
       ----------------------

       This excellent book is offered to the public by the
       author:

          Clive G. Page,
          Professional Programmer's Guide to Fortran 77
          Pitman, 1988
          122 pages (including index)


       It can be found at the anonymous FTP site:

          Host:       ftp.star.le.ac.uk
          Directory:  /pub/fortran/
          File:       prof77.ps.gz

       There is also a Latex version available.


       -----------------------------------------------
       ~From: Z.W.T.Mason@sussex.ac.uk (Zebedee Mason)
       -----------------------------------------------

       Jeffrey Templon (templon@studbolt.mit.edu) wrote:
       : Hi,
       :
       : I just discovered this one and don't remember seeing it pointed
       : to here. It's a PS copy of an out-of-print book by Clive Page,
       : "Professional Programmer's Guide to Fortran 77" and what I've
       : seen of it looks real good.
       :
       :                                                JT

       I bought it when it was in print, never needed to buy another
       one since. Why can't all programming books be this short and
       to the point?

          Zeb.



       Another free Fortran 77 book
       ----------------------------

       Interactive Fortran 77: A Hands on Approach (second edition)
          Ian D Chivers and Jane Sleightholme
          Ellis Horwood, 1990
          Series in Computers and their Applications
          ISBN: 0-13-466764-6

       Copyright (C) Ian D Chivers and Jane Sleightholme.

       Legal comments:

          Unless otherwise specified, Ian D Chivers and Jane Sleightholme
          hold all rights, including copyright and retains such rights.
          This work may be distributed in its entirety provided the work
          is distributed as a whole with this copyright notice intact.

          This work may not be distributed in hard copy or other machine
          readable form, redistributed, transmitted or translated without
          prior written authorization from Ian D Chivers and Jane Sleightholme.

          Commercial use can only be allowed by specific license agreements.
          The accuracy of this document cannot be guaranteed. Ian D Chivers
          and Jane Sleighthome make no warranty, either express or implied,
          with respect to the use of any information and assumes no liabilities
          for loss or damage, whether such loss or damage is caused by error
          or omission.

          If this electronic book is made available anywhere other than the
          original system, Ian Chivers or Jane Sleigtholme must be notified
          in writing (email is acceptable) and the copyright notice must
          retain intact.

       PDF version:

          http://www.kcl.ac.uk/kis/support/cc/fortran/f77book.pdf

       Unix compressed postscript version:

          http://www.kcl.ac.uk/kis/support/cc/fortran/f77book.ps.Z

       PC pkzip postscript version:

          http://www.kcl.ac.uk/kis/support/cc/fortran/f77ps.zip


   __________________________________________________________________________
                                       


1.2.2) Where can I find a f90 tutorial or course?

       Copyright but freely available course material is available
       from Manchester Computer Centre on the World Wide Web with
       the URL:

          http://www.hpctec.mcc.ac.uk/hpctec/courses/Fortran90/F90course.html

       The ftp address is:

          host:       ftp.mcc.ac.uk
          directory:  /pub/mantec/Fortran90



       A complete Tutorial is available under WWW with
       the URL:

          http://asis01.cern.ch/CN/CNTUT/f90/Overview.html

       or via anonymous ftp from:

          host:       cernvm.cern.ch
          directory:  cnl.200
          file:       f90tutor.ps

       An ASCII copy of this material as a set of slides for a
       six-hour course is available from:

          metcalf@cern.ch.



   Courses are available from:


       Walt Brainerd, a member of X3J3,
          also on HPF
          email:  walt@fortran.com

       PSR (see above);

       CETech, Inc. (also on HPF)
          8196 SW Hall Blvd., Ste. 304,
          Beaverton, Oregon 97008, USA.
          Phone:  (503)644-6106
          Fax:    (503)643-8425
          Email:  cetech@teleport.com).

    Some European companies offering courses and conversion
    consultancy are:

       IT Independent Training Limited,
          113 Liscombe, Birch Hill,
          Bracknell, Berkshire, RG12 7DE, UK
          tel:  +44 344 860172
          fax:  +44 344 867992


       Simulog, attn. Mr. E.Plestan,
          1 rue James Joule,
          F-78286 Guyancourt Cedex, France
          tel:  +33 1 30 12 27 00
          fax:  +33 1 30 12 27 27


       CTS,
          Prinz-Otto Str. 7c,
          D-85521 Ottobrunn , Germany
          tel:  +49-89-6083758
          fax:  +49-89-6083758


   __________________________________________________________________________
                                       


1.2.3) What constitutes good FORTRAN style?

       One rendition of a FORTRAN 77 style guide is available through
       anonymous ftp from ics.uci.edu (128.195.1.1).  To retrieve
       (please note that it's not really "anonymous", that's just
       the Name that you'll be using):

          % ftp ics.uci.edu
          anonymous <enter your e-mail address at Password: prompt>
          cd pub/levine
          ascii
          get F77_Style_Guide
          bye

       If you can't access this site directly, please send an e-mail
       request to:

          INTERNET:   levine@ics.uci.edu
          BITNET:     levine@uci
          UUCP:       ...!uunet!ucivax!levine


   __________________________________________________________________________
                                       


1.2.4) What are good Subsets of Fortran?

One is F:

       Announcing the first book on the F programming language
       -------------------------------------------------------

       "The F programming Language", by Michael Metcalf and John Reid,
       Oxford University Press, Oxford and New York, 1996,
       ISBN 0-19-850026-2, (about $US30 or 16.95 pounds sterling).

       The F programming language is a dramatic new development in
       scientific programming. Building on the well-established strengths
       of the Fortran family of languages, it is carefully crafted to be
       both safe and regular, whilst retaining the enormously powerful
       numerical capabilities of its parent language, Fortran 90, as well
       as its data abstraction capability. Thus, an array syntax becomes
       available as part of a medium-size, widely-available language for
       the first time. In this respect, the language is clearly superior
       to older ones such as Pascal, C, and Basic.

       F is ideally suited for teaching as a first programming language,
       and provides a smooth path into both Fortran 90 and High Performance
       Fortran (it is a subset of both).

       In the absence of a formal standard for F, this book is the defining
       document for the language, setting out the complete syntax and
       semantics of the language in a readable but thorough way.
       It is essential reading for all F practitioners.

       Compilers for F are available from Imagine1 for Windows 95, Linux
       and some Unix platforms, with Windows NT, Macintosh PowerPC and 68K
       families coming shortly. The compilers are based on technology from
       Absoft,  Fujitsu, and NAG. For details see:

          http://www.imagine1.com/imagine1 or contact info@imagine1.com.


          Table of Contents:
          1.  Why F? . . . . . . . . . . . . . . . .  1
          2.  Language elements  . . . . . . . . .    7
          3.  Expressions and assignments  . . . .   29
          4.  Control constructs   . . . . . . . .   49
          5.  Program units and procedures   . . .   61
          6.  Array features   . . . . . . . . . .   89
          7.  Specification statements   . . . . .  113
          8.  Intrinsic procedures   . . . . . . .  131
          9.  Data transfer  . . . . . . . . . . .  151
          10. Operations on external files   . . .  175
          Appendix A.  Intrinsic procedures  . . .  185
          Appendix B.  The statements of F . . . .  191
          Appendix C.  Diffences from Fortran 90 .  195
          Appendix D.  Pointer example   . . . . .  201
          Appendix E.  The terms of F  . . . . . .  211
          Appendix F.  Solutions to exercises  . .  221
          Index  . . . . . . . . . . . . . . . . .  233


       Michael Metcalf works at CERN, Geneva. He is the author of a
       range of publications, including the books "Effective Fortran 77"
       and "Fortran 90/95 Explained" (with John Reid) (Oxford University
       Press), and "Fortran Optimization" (Academic Press).
       He was Editor of the Fortran 90 standard.

       John Reid works for the Rutherford Appleton Laboratory and
       is well known as a numerical analyst; he is a co-author of
       "Direct Methods for Sparse Matrices" and "Fortran 90/95 Explained"
       (Oxford University Press). He served as Secretary of X3J3 and
       played a leading role in the development of Fortran 90.


   Ordering information:

       1) N. America: Order Department, Monday-Friday, 8:15am-5:00pm (EST)

             Phone:   1-800-451-7556
             Fax:     1-919-677-1303
             Post:    Order Department
                      Oxford University Press
                      2001 Evans Road
                      Cary, NC 27513
             E-mail:  orders@oup-usa.org
             WWW:     http://www.oup-usa.org/

       2) UK: send order and payment to:

             CWO Department, OUP,
             FREEPOST NH 4051, Corby, Northants
             NN18 9BR - no stamp required

             Phone: with a credit card, the 24-hour credit
                    card hotline is:  +44 (0)1536 454534

             Postage and packing for UK orders:
                    - under #20 - add #2.06,
                      over #20 - add #3.53,
                      over #50 - add #4.70.

             WWW: http://www.oup.co.uk/

       3) Eire, Europe, and the rest of the world,
          send order and payment to:

            CWO Dept, OUP,
            Saxon Way West, Corby,
            Northants NN18 9ES, UK

          Fax:  credit card sales: +44 1536 746337

          Postage and packing for non-UK orders:
            add 10% of the total price of the books.

       4) Imagine1
          11930 Menaul NE, Suite 106
          Albuquerque, NM 87112
          Toll free phone number: 1 888 323 1758.
          See also Imagine1's e-mail address and WWW URL above.

   Demos available (and free for linux)

          ftp  swcp.com
          login as anonymous and give e-mail address as password
          cd  ~ftp/pub/walt/Fbin
          get f_linux.tar.Z  (or f_solaris1.tar.Z or f_solaris2.tar.Z)

       Please send problems or questions to
       info@imagine1.com.
       --------

Another subset is ELF,

       Lahey has a native LF90 compiler for Windows and DOS:

          sales@lahey.com
          http://www.lahey.com

       It is particularly well optimized on the Pentium.

       Also on offer is elf90, a subset language that does not have old
       features like storage association, is designed for teaching, and is
       very cheap.  Also "Prof. Loren Meissner" <meissner@usfca.edu>
       can provide information, and possibly a textbook on this dialect.
       But in a nutshell, elf90 is said to be f90 sans What's not in Elf90

       To promote a more efficient and modern programming language the
       Fortran  statements listed below are not supported by the Elf90
       language. If you use  a Fortran 90 feature that is not supported, an
       on-screen error message is  provided.

          ALLOCATABLE*        ASSIGN              BLOCK DATA
          COMMON              CONTINUE            DATA DIMENSION*
          DO LABEL            DOUBLE PRECISION    END
          END BLOCK DATA      ENTRY               EQUIVALENCE
          EXTERNAL            GO TO (COMPUTED)    GO TO (ASSIGNED)
          IMPLICIT            INCLUDE             INTENT*
          INTRINSIC           OPTIONAL            PARAMETER*
          POINTER*            SAVE*               TARGET*

       *Note: The ALLOCATABLE, TARGET, POINTER, INTENT, PARAMETER,
       DIMENSION, and  SAVE attributes are declared in type declaration
       statements.

       <khb note: elf90 is, as I understand it, available on Intel
       processors only. F is said to be (or soon to be) available on a
       variety of processors, including Intel, SPARC and Macintosh.>


   __________________________________________________________________________
                                       


1.3) General Fortran (particularly Fortran 90) resources



1.3.1) f90.faq


       Michel Olagnon's Fortran 90 List
       --------------------------------

       F90 FAN's : Fortran 90 Frequently Asked about News.
       A Fortran 90 addition to the Fortran FAQ.

       Michel Olagnon - October 1st, 1993.
       Last updated - November 29th, 1996.

       Send flames and suggestions for improvement to:

          email:  Michel.Olagnon@ifremer.fr
          WWW:    http://www.ifremer.fr/ditigo/molagnon/molagnon.html

       The current updated version of this FAQ is available
       from:

          ftp://ftp.ifremer.fr/ifremer/ditigo/fortran90/engfaq

       It can be found on WWW at URLs:

          http://www.mols.susx.ac.uk/eggen/Fortran90/f90-faq.html
          (thanks to Bernd Eggen),

          http://www.kcl.ac.uk/kis/support/cc/fortran/engfaq.html
          (thanks to Ian Chivers),

          http://lenti.med.umn.edu/~mwd/f90-faq.html
          (thanks to Mark Dalton),

          http://www.uni-karlsruhe.de/~Fortran90/olagnon-faq.html
          (thanks to Michael Hennecke),

          http://www.ifremer.fr/ditigo/molagnon/fortran90/engfaq.html


       Contents :
       ----------

       1. Fortran 90 and Fortran 77
       2. Available in Fortran 90:

          2.1. Compilers
          2.2. Code re-structurers and converters
          2.3. Libraries and utilities
          2.4. Tests and Benchmarks
          2.5. Examples and repositories
          2.6. Courses and Consultancy

       3. Documentation:

          3.1. Standards
          3.2. Glossary
          3.3. Journals
          3.4. Tutorials and other documents
          3.5. Books
          3.6. Articles
          3.7. WWW-Mosaic pages

       4. Fortran 90 Benchmarking
       5. Announced, foreseen, and rumours
       6. Workshops, seminars, conferences
       7. Developments, related languages

          7.1. Standard
          7.2. HPF
          7.3. PVM
          7.4. MPI
          7.5. Parallel Programming

       8. Addresses


   1.0 Fortran 90 and Fortran 77:
   ------------------------------

       Fortran 90 is, with very few exceptions, a superset of Fortran 77.
       The FAQ of the Usenet group Comp.lang.fortran deals with both
       standards, and may be obtained, like any FAQ, via anonymous ftp
       from:

          ftp://rtfm.mit.edu/pub/usenet/comp.lang.fortran/Fortran_FAQ

          host:       rtfm.mit.edu
          directory:  pub/usenet/comp.lang.fortran
          file:       Fortran_FAQ

       It is also available on the WWW:

          http://www.cis.ohio-state.edu/hypertext/faq/usenet/
                                         fortran-faq/faq.html

       The present document is an attempt to supplement that FAQ with
       some specific Fortran 90 information.

       Anyone interested is also invited to join the mailbase list
       comp-fortran-90, by sending an e-mail message to:

          mailbase@mailbase.ac.uk

       containing the only line:

          join comp-fortran-90 firstname  lastname

       more info on URL:

          http://www.mailbase.ac.uk/lists-a-e/comp-fortran-90/



       The main extensions of Fortran 90 over Fortran 77 are:
       ------------------------------------------------------

       o  array notation (for instance, X(1:N)=R(1:N)*COS(A(1:N)))
       o  dynamic memory allocation (ALLOCATE, DEALLOCATE, ...)
       o  derived types and operator overloading
       o  better declarations, and prototyping possible
       o  MODULES, allowing users to create ``storage pools'',
          or to define environment
       o  more of modern control structures (SELECT CASE, EXIT, ...)
       o  more of useful intrinsics (date, precision, arrays, ...)
       o  free format source code form


       ``Pure'' Fortran 77 is F90 compatible. Yet, it is better to convert
       it to a ``mixed'' format, acceptable both as free and fixed source
       form Fortran 90, which only requires replacing C by ! as the comment
       character, to use & as the continuation line character, and to
       append it to the continued line, to remove blanks embedded inside
       constants or identifiers, and to check some intrinsics usage. Most
       of this can be done automatically.

       Fortran 90 allows the Fortran 77 programmer to write code faster,
       to make it more legible, and to avoid many bugs. For a newcomer to
       programming, it is an opportunity to learn a modern language, with
       most recommended features, and yet to be in line with scientific
       and industrial engineering communities where Fortran is and is
       going to remain for a good while THE favourite language.



   2.0 Available in Fortran 90:
   ----------------------------

       2.1 Compilers
       -------------

       There is presently no free full F90 compiler. However, some
       compilers restricted to modern subsets of the language are free.
       These are:

          ELF90 from Lahey
             for DOS 3.3 or higher, Windows 95, or Windows NT:

             http://www.lahey.com/"


          F from Imagine1 for Linux:

             http://www.imagine1.com/imagine1

       Compilers for these subsets are also available for other
       platforms, but presently not for free.



       Absoft's version of CF90
          for:  Power Mac
          URL:  http://www.absoft.com

       ACE f90 and HPF
          for:  Parsytec PowerPC-based machines
          URL:  http://www.ace.nl/

       Apogee - highly optimizing Apogee-Fortran 90, C-DAC Fortran 90
          (comes with debugger).
          Both compilers are for SPARC architectures.
          URL:  http://www.apogee.com/

       APR xHPF 2.1 - HPF compiler
          ([Cray]T3D,
           [IBM]SP-2,
           [Intel]Paragon,
           [Dec Alpha]3000/900 275Mhz,
           [SGI Power Challenge]MIPS R8000,
           [Sun SPARC]2000 40Mhz)

       CRAY CF90
          for:  Crays YMP and YMP-C90,
                Superserver 6400
                Sparc Solaris 2.3
          plans for HP, SGI
          URL:  http://www.cray.com/PUBLIC/product-info/craysoft/
                                                  Fortran_90.html

       DEC Fortran 90 V2.0
          for:  Digital UNIX Alpha
                OpenVMS Alpha,
          UNIX version including full HPF support, Digital Parallel
          Software Environment (PSE), companion product on UNIX for
          HPF programming.
          URL:  http://www.digital.com/info/hpc/f90

       EPC Fortran 90
          for:  Sparc Solaris 1.X and 2.X,
                IBM RS/6000,
                Intel 3/486 (SVR3&4, Solaris 2.x),
                SGI,
                Motorola 88000/100/100 (SVR3&4),
                MIPS

       Fujitsu full compiler
          for:  Sparc Solaris 1.1 and 2.x
          next: Sun Sparc (MP) 3Q/95,
                HP PA-RISC 4Q/95
                MIPS ABI 4Q/95,
                SGI 4Q/95,
                Windows 1Q/96

       HP, HP Fortran 90 - full compiler
          for:  HP-UX 10.20,
                      10.10,
                      10.01
                SPP-UX
          URL:  http://www.hp.com/go/hpfortran

       IBM XLF V3 full compiler
          for:  RISC System/6000 + KAP preprocessor
          from KAI, for AIX V3.2 and V4.1
          URL:  http://www.torolab.ibm.com:80/ap/fortran/xlfortran/

       Imagine1 F - educational subset
          (dusty features removed, for inexpensive F90 learning)
          URL:  http://www.imagine1.com/imagine1

       Lahey LF90
          for:  DOS,
                Windows including Pentium optimizations and
                   Interacter Kit.
          URL:  http://www.lahey.com/

       Lahey ELF90 - educational subset
          (dusty features removed, for inexpensive F90 learning)

       Microsoft Fortran Powerstation V4.0
          for:  Windows NT 3.5
                Windows 95
          URL:  http://www.microsoft.com/fortran

       MicroWay
          for:  DOS,
                OS/2,
                Unix,
                Linux.

       NA Software F90+
          for:  OS/2,
                DOS/Windows3.1,
                Windows NT,
                Sun,
                Inmos T800
                PC Linux, also HPF for Linux.
          Cost-effective personal version for Windows95
          URL:  http://www5.informatik.tu-muenchen.de/sci-comp/info/
                                               software/fortran.html

       NAG/ACE Optimizing f90 - release 1.0
          for:  Sparc Solaris 2.
          URL:  http://www.nag.co.uk/nagware/ACE/Info.html

       NAGWare f90
          uses C as intermediate language, now at rel:2.2,
          includes HPF extensions and exists in Linux version.
          URL:  http://www.nag.co.uk/nagware/NCNJNKNM.html

       NEC FORTRAN90/SX
          for its supercomputer SX series.

       Pacific Sierra VAST/f90
          uses F77 as intermediate language,
          for:  Unix
                VMS
                Convex
          URL:  http://www.psrv.com/vast/vastf90.html

       Parasoft
          uses F77 as intermediate language
          URL:  http://www.parasoft.com/f90.html

       PGI f90/HPF compiler,
          for:  SGI,
                IBM SP2,
                HP/Convex
          URL:  http://www.pgroup.com/

       Salford FTN90
          PC implementation of NAG f90, direct generation
          of object code.
          URL:  http://www.salford.ac.uk/docs/ss.html

       SGI
          under IRIX 6.1 on R8000 machines:
             Power Challenge,
             Power Indigo 2,
             Power Onyx
          URL:  http://www.sgi.com/

       SPARCompiler Fortran 90
          Sun's Cray-compatible compiler.
          URL:  http://www.sun.com/sunsoft/Products/Developer-products

       Stern C. S. CF90
          Cray-compatible for DEC OSF/1 (Digital UNIX).


       NOTE:  Some vendors, such as Convex on their machines, offer
              a number of F90 extensions, for instance array syntax
              or ALLOCATE instruction.



       Code re-structurers and converters
       ----------------------------------

       Pacific-Sierra VAST/77to90
          (see article by JKP in Fortran Journal 5/4)
          URL:  http://www.psrv.com/vast/vast77to90.html

       LOFT90, by NA Software
          (available also under Linux)

       FORESYS 1.4
          GUI based High Performance Global Analysis,
          F77->F90 conversion, and parallelization.
          URL:  http://www.cais.net/s2i/www/general/foresys.html

       FORGE Explorer 2.0
          Distributed and shared memory Parallelizer,
          Applied Parallel Research, Inc.
          URL:  http://www.infomall.org/apri/

       NAGWare f90 tools
          pretty-printer,
          declarations standardiser,
          precision standardiser,
          names changer.
          URL:  http://www.nag.co.uk/nagware/NENF.html

       CONVERT, conversion to F90 free format
          proposed by Mike Metcalf via anonymous ftp
          on:
             host:       jkr.cc.rl.ac.uk (130.246.8.23)
             directory:  pub/MandR/
             file:       convert.f90
          URL:  ftp://jkr.cc.rl.ac.uk/pub/MandR/convert.f90

       ftof90.c
          minimal F77 -> F90 conversion.
          URL:  ftp://ftp.ifremer.fr/ifremer/ditigo/fortran90/ftof90.c.gz

       f90ppr
          F90 pre-processor similar to cpp.
          URL:  ftp://ftp.ifremer.fr/ifremer/ditigo/fortran90/f90ppr.f90.gz

       flecs90
          FLECS to F90 translator.
          URL:  ftp://odin.mda.uth.tmc.edu/pub/source/flecs90.tar.Z

       HPF mapper
          for PVM or Parmacs,
          on Sun clusters: NA software.



       Libraries and utilities
       -----------------------

       *Emacs* package free-format f90-mode
          URL:  http://www.mailbase.ac.uk/lists-a-e/comp-fortran-90/
                                                        files/f90.el
          Among the options one finds automatic matching and completion
          of all end-blocks (for example, indenting a line starting with
          end, finds the corresponding if/do/module... and checks/fills
          in the right kind of block and a possible name), it has an
          automatic fill-function which breaks a line and inserts
          &-signs (two if inside a string) when a line gets too long,
          different coloring for different features which is updated
          with every indent of a line.
          The most common commands are available via a menu.

       Performance Library
          LAPACK, BLAS, FFTPACK, VFFTPACK et LINPACK
          optimized for SPARC (Sun Performance Workshop).
          URL:  http://www.sun.com/sunsoft/Products/Developer-products

       INTERACTER
          graphics library for Lahey LF90 and Salford FTN90,
          on 386/486/pentium + DOS Extenders (Int. Soft. Serv.).
          URL:  http://www.demon.co.uk/issltd/

       Lahey has F90 components (manual, array intrinsics, front end,...)
          that they would like to license to others.

       NAG fl90, numerical and statistical library,
          Sun 4, Sgi, DECstation, and IBM RISC System/6000.

       NAG tool components
          (parser, semantic analyser, tree modification library
          and tree flattener).

       Numerical recipes
          URL:  http://nr.harvard.edu/nr/nrf90_blurb.html
          (Others give caveats:  http://math.jpl.nasa.gov/nr !)

       Cray LibSci(tm),
          numerical library for Crays and Sparc Solaris 2.3

       MPFUN
          (Multiple Precision Floating Point Computation Package)
          by David W. Bailey, for Cray CF-90.
          URL:  ftp://ftp.irisa.fr/pub/netlib/mpfun/

       MSL library (Visual Numerics)

       Syntax verifier extracted from NAG compiler,
          put into public domain by NAG for Sun 3, Sun 4, Sgi.
          Interactive checking of user's code over www at:
          URL:  http://www.nag.co.uk/0/Forms/f90_interface.html

       ISF and PKF modules
          shareware from Garnatz and Grovender, Inc
          ISAM/VSAM/btree file structure, and Positional Key file structure
          URL:  http://www.winternet.com/~gginc

       XLIB interface
          from Garnatz and Grovender also.
          URL:  http://www.winternet.com/~gginc

       CADNA,
          by professeur Vignes from Universite Pierre et Marie Curie,
          implements stochastic arithmetic in Fortran 90, and
          enables monitoring of precision loss and/or numerical
          instabilities during execution. (Control of Accuracy
          and Debugging for Numerical Aplications in Fortran)
          More information available from AERO (see also articles
          by J. Vignes), or Pr. Chesneaux (chesneaux@masi.ibp.fr).

       ISO/IEC 1539-2 (Auxiliary standard)
          Variable length character strings in Fortran
          (with a demonstration of implementation at URL:
           ftp://ftp.liv.ac.uk/pub/fortran_std/is1539-2.html)

       LAPACK,
          (minimaly) translated by myself (M.O.), successfully
          passed all its tests with NAg-f90 2.0.
          I aggressively translated single precision Blas, and
          intend to do the same with other Blas as soon as I
          have time.
          Steve Moulton works on LAPACK conversion.

       StopWatch
          Measurement of execution times by W.F Mitchell
          URL:  http://math.nist.gov/acmd/Staff/WMitchell/StopWatch.html

       F90 makedepend
          perl script by Kate Hedstrom
          URL:  http://marine.rutgers.edu/po/perl.html

       Automatic differentiation with Fortran programs
          URL:  http://www.mcs.anl.gov/Projects/autodiff/AD_Tools



       Tests and Benchmarks
       --------------------

       Lahey Test suite
          F77 & F90 (license agreement)

       NAGware Test suite
          tests for compilers (same as U_F90_TS)

       U_F90_TS Test suite
          from Dr. Brian Smith (University of New Mexico),
          marketed by Unicomp and NAG.

       SHAPE Test suite
          3400 tests of array instructions,
          from Spackman & Hendrickson, Inc.

       Parasoft Test suite
          1500 tests for compilers

       Quetzal Benchmark
          from John K. Prentice.
          URL:  http://www.swcp.com/~quetzal/access.html

       Benchmark of Syracuse University
          via anonymous ftp on:
             host:       minerva.npac.syr.edu
             directory:  old_pub
          URL:  ftp://minerva.npac.syr.edu/old_pub/

       Channel benchmark
          by John D. McCalpin, via anonymous ftp on:
             host:       perelandra.cms.udel.edu
             directory:  bench/channel.
          URL:  ftp://perelandra.cms.udel.edu/bench/channel



       Examples and repositories
       -------------------------

       Nag has set up a repository for contributed code:
          WWW:  http://www.nag.co.uk/1/nagware/Examples

       The Fortran Market has established itself on the World Wide Web.
          "ONE place to find all information, products,
          and services related to Fortran"
          WWW:  http://www.fortran.com/fortran/market.html

       Lahey Computer Systems
          downloadable F90 public domain code.
          URL:  http://www.lahey.com/other.htm

       11,000 lines offered by Richard Maine via anonymous ftp on:
          host:       ftp.dfrf.nasa.gov
          directory:  pub/fdas/f90sample/
          file:       fdas.tar.Z

       Many of the example codes and problem solutions from:
          NUMERICAL METHODS FOR DIFFERENTIAL EQUATIONS -
          A computational approach, by John R. Dormand
          have been coded in F.
          URL:  ftp://ftp.tees.ac.uk/pub/j.r.dormand/F-files

       STEJOI, statistical package for joint occurrence events,
          on Sun, including source code and everything,
          via anonymous ftp on:
          host:       ftp.ifremer.fr
          directory:  ifremer/ditigo/fortran90/
          file:       f90dvl.tar.Z

       Module unsigned_32
          for definition and use of unsigned 32 bits integers,
          also via anonymous ftp on:
          host:       ftp.ifremer.fr
          directory:  ifremer/ditigo/fortran90/
          file:       unsi32.f90.Z

       f90split, experimental version,
          similar to Unix BSD fsplit, but for free source form,
          also via anonymous ftp on:
          host:       ftp.ifremer.fr
          directory:  ifremer/ditigo/fortran90/
          file:       f90split.f90.gz

       Algorithm 999 by A.G. Buckley
          for unconstrained nonlinear minimization,
          via anonymous ftp on:
          host:       ftp.royalroads.ca
          directory:  pub/software/bbuckley/alg999/
          file:       source



       Courses and Consultancy
       -----------------------

       IT Independent Training Limited, UK

       CTS, Germany

       Unicomp, USA

       Pacific-Sierra Research Corp., USA

       CETech, Inc., USA



   3.0 Documentation:
   ------------------


       Standards
       ---------

       ISO/IEC 1539:1991 (E) International Standard
          Information technology - Programming langages - Fortran
          Somewhat expensive (CHF 210 ~ US$ 140 !) for instance, at ISO.
          Surprisingly enough, the identical, save for foreword and
          acknowledgements, ANSI standard X3.198-1992 is even more expensive.

          Walter S. Brainerd, Unicomp., offers:

             o  for 125 US$, an electronic ascii monouser version,
             o  for 125 + 10n US$, an electronic PostScript version,
                and the right to make n paper copies,
             o  or for 1000 US$, an electronic ditroff monouser version.

          URL:  http://www.fortran.com/fortran/iso1539.html

          A version with French glossary is available as European norm
          NF EN 21539.



       Glossary
       --------

       Fortran terminology glossary
          by Ken Hawick hawick@npac.sys.edu
          URL:  http://www.npac.syr.edu/hpfa/fortgloss/fortgloss.html



       Journals
       --------

       Fortran Journal
          ISSN 1060-0221
          Enquiries: Walt Brainerd  (email:  walt@fortran.com)
          Subscriptions:  Fortran Users Group
                          P.O. Box 4201
                          Fullerton, CA 92634
          (about $30/year individual, $100/year company,
           ~$50/$150 outside the USA, call 1 (714) 441 2022)

       Fortran Forum
          edited by Loren Meissner (email:  meissner@usfca.edu)
          Subscriptions:  ACM membership services
                          email:  acmhelp@acm.org
                          10$ members, 20$ non members
          More info:  http://www.acm.org/



       Tutorials and other documents
       -----------------------------

       University of Liverpool on-line tutorial
          URL:  http://www.liv.ac.uk/HPC/HTMLFrontPageF90.html

       P. Corde and H. Delouis
          ``Support de cours Fortran 90 IDRIS''.
          This is a very complete reference (224 pp.), in French,
          for which the authors have agreed to give free access.
          URL:  http://www.idris.fr/data/cours/lang/f90/F90_cours4.ps

       Prof. Loren Meissner has written an ELF subset
          (Essential Lahey Fortran) textbook, from his PWS book,
          and offers it on a royalty basis of $1.00 per copy,
          with advance royalty payment for 100 copies
          (email:  LPMeissner@msn.com).

       Copyright but freely available course material
          is available from Manchester Computer Centre.
          URL:  http://www.hpctec.mcc.ac.uk/hpctec/courses/Fortran90/
                                                       F90course.html

       Bo Einarsson and Yurij Shokin
          have written a tutorial on the transition from
          Fortran 77 to Fortran 90, with the title:
             "Fortran 90 for the Fortran 77 programmer"
          URL:  http://www.nsc.liu.se/f77to90.html

       Michel Goossens has now installed a Fortran 90 tutorial
          on the World Wide Web (WWW), with the title:
             "F90 Tutorial/Overview"
          There is no copyright on this material.
          URL:  http://wwwcn.cern.ch/asdoc/f90.html

       There is a Fortran (90) tutorial on the net that might
          be of some use (from the University of New Mexico).
          URL:  ftp://mycroft.plk.af.mil/pub/Fortran_90/Tutorial/

       See also:

          URL:  http://www.nsc.liu.se/~boein/fortran.html

          URL:  http://www.kcl.ac.uk/kis/support/cc/fortran/f90home.html

          Digital Equipment Corporation (DEC)
             URL:  http://www.digital.com:80/info/hpc/f90/users.html#tutorial

          Computational Science Education Project (CSEP)
             Oak Ridge National Laboratory (ORNL)
             URL:  http://csep1.phy.ornl.gov/pl/pl.html

          URL:  ftp://ftp.th-darmstadt.de/pub/thd/fortran/f90/

          The University of Liverpool
             URL:  http://www.liv.ac.uk/HPC/F90page.html

          Belfast
             URL:  http://www.pcc.qub.ac.uk/tec/courses/courselist.html

          Univ. of New Mexico
             URL:  http://www.arc.unm.edu/workshop/fortran90/f90-main.html

          Syracuse Univ.
             URL:  http://www.npac.syr.edu/EDUCATION/PUB/hpfe/

          Pacific-Sierra Research mini-tutorial about converting
             Fortran 77 programs to High Performance Fortran
             URL:  http://www.psrv.com/77toHPF

          EPCC Writing Data parallel programs with High Performance Fortran
             URL:  http://www.epcc.ed.ac.uk/epcc-tec/package.html

          Leicester
             URL:  ftp://ftp.star.le.ac.uk/pub/fortran/



       Books
       -----

   * in English,

       Adams, Brainerd, Martin, Smith.
          Fortran Top 90 - Ninety Key Features of Fortran 90,
          Unicomp, Sept. 1994.

       Adams, Brainerd, Martin, Smith, Wagener.
          Fortran 90 Handbook,
          McGraw-Hill, 1992.
          ISBN 0-07-000406-4

       Brainerd, W., Goldberg, and Adams.
          Programmer's guide to Fortran 90,
          2nd edition, Unicomp, 1994.
          ISBN 0-07-000248-7

       Chamberland, Luc.
          Fortran 90 : A Reference Guide,
          Prentice Hall.
          ISBN 0-13-397332-8.

       Chivers, I. and Sleightholme, J.
          Introducing Fortran 90,
          Springer-Verlag, Sept. 1995.
          ISBN 3-540-19940-3
          URL:  http://www.kcl.ac.uk/kis/support/cc/fortran/

       Counihan,
          Fortran 90,
          Pitman, 1991.
          ISBN 0-273-03073-6

       Einarsson, B., Shokins, Y.
          Fortran 90 for the Fortran 77 programmer
          HTML-book.
          URL:  http://www.nsc.liu.se/~boein/fortran.html

       Ellis, T.M.R, Lahey, T. and Philips, I.
          Fortran 90 Programming,
          Addison Wesley, 1994,
          ISBN 0-201-54446-6
          With examples in URL:
             ftp://aw.com/aw.computer.science/

       Gehrke, W.
          Fortran 95 Language Guide,
          Springer-Verlag, 1996.
          ISBN 3-540-76062-8 (Softcover)

       Hahn, B.D., Edward Arnold.
          Fortran 90 for Scientists and Engineers,
          1994.
          ISBN 0-340-60034-9

       Kerrigan, J.
          Migrating to Fortran 90,
          O'Reilly and Associates, 1993 (2nd ed. Sept.94),
          ISBN 1-56592-049-X
          With examples in URL:
             ftp://uunet.uu.net/nutshell/fortran90/

       Charles H. Koelbel, David B. Loveman, Robert S. Schreiber,
          Guy L. Stelle Jr., Mary E. Zosel
          High Performance Fortran Handbook,
          MIT Press, 349 pages, 1994.
          ISBN 0-262-61094-9  $24.95 in paper back
          ISBN 0-262-11185-3  $45 for hard cover

       Mayo, W.E. and Cwiakala, M.
          Schaum's Outline of Theory and Praxis
          -- Programming in Fortran 90,
          Mc Graw Hill, 1996.
          ISBN 0-07-041156-5

       Meissner, L.
          Fortran90,
          PWS Kent, Boston, 1995.
          ISBN 0-534-93372-6

       Metcalf, M. and Reid, J.
          Fortran 90/95 Explained,
          Oxford University Press, 1996.
          ISBN 0-19-851888-9

       Metcalf, M. and Reid, J.
          The F programming Language,
          Oxford University Press, 1996.
          ISBN 0-19-850026-2

       Morgan and Schonfelder,
          Programming in Fortran 90,
          Alfred Waller Ltd., 1993.
          ISBN 1-872474-06-3

       Redwine, C.,
          Upgrading to Fortran 90,
          Springer, 1995
          ISBN 0-387-97995-6

       Schick W., Silverman Gordon,
          Fortran90 and engineering computations,
          John Wiley and sons, 1995
          ISBN 0-471-58512-2

       Smith, I.M.
          Programming in Fortran 90,
          Wiley,
          ISBN 0-471-94185-9
          With examples in URL:
             ftp://golden.eng.man.ac.uk/pub/fe/

       Vowels, R.
          Introduction to Fortran 90/95, Algorithms and
          Structured Programming
          ISBN 0-9596384-8-2
          URL:  http://www.cs.rmit.edu.au/~rav/FORTRAN.html


   * in French,


       Aberti, C.
          Fortran 90: Initiation a partir du Fortran 77,
          S.I. E'ditions, 1992.
          ISBN 2-909615-00-6

       Ain, M.
          Savez-vous parler Fortran,
          Bibliotheque des universites (de Boeck), 1994.
          ISBN 2-8041-1755-3

       Delannoy, C.
          Programmer en Fortran 90,
          Eyrolles, 1992.
          ISBN 2-212-08723-3

       Dubesset, M. et Vignes, J.
          Les spe'cificites du Fortran 90,
          E'ditions Technip, 1993.
          ISBN 2-7108-0652-5

       Lignelet, P.
          Fortran 90: Approche par la Pratique,
          S.I. E'ditions, 1993.
          ISBN 2-909615-01-4

       Lignelet, P.
          Manuel complet du langage Fortran 90 et Fortran 95,
          Calcul intensif et ge'nie logiciel,
          Masson, 1996.
          ISBN 2-225-85229-4

       Lignelet, P.
          Structures de Donne'es (et leurs algorithmes) en Fortran 90/95
          Masson, 1996.
          ISBN 2-225-85373-8
          URL:  http://www.ifremer.fr/ditigo/molagnon/fortran90/livrepl2.html

       Metcalf, M. et Reid, J.
          (translated by M. Caillet and B. Pichon)
          Fortran 90: Les concepts fondamentaux,
          AFNOR Editions, 1993.
          ISBN 2-12-486513-7

       Olagnon, M.
          Traitement de donne'es nume'riques avec Fortran 90
          Masson, 1996.
          ISBN 2-225-85259-6
          URL:  http://www.ifremer.fr/ditigo/molagnon/livre.html


   * in Chinese,


       He Xingui, Xu Zuyuan, Wu Gingbao and Chen Mingyuan
          Programming Language FORTRAN 90,
          China Railway Publishing House, Beijing, 1994.
          ISBN 7-113-01788-6/TP.187


   * in German,


       Brainerd, W.S., Goldberg Ch.H., Adams J.C.,
          (translated by Peter Thomas and Klaus G. Paul)
          Fortran 90, Lehr- und Arbeitsbuch fuer das erfolgreiche Programmieren
,
          R. Olbenbourg Verlag, Muenchen, 1994,
          ISBN 3-486-22102-7

       Gehrke.
          Fortran 90 Referenz-Handbuch,
          Carl Hansen Verlag, 1991.
          ISBN 3-446163-21-2

       Heisterkamp.
          Fortran 90: Eine Informelle Einfuehrung,
          BI-Wissenschaftsverlag, 1991.
          ISBN 3-411153-21-0

       Langer.
          Programmieren in Fortran,
          Springer Verlag, 1993.
          ISBN 0-387-82446-4

       Michel, T.
          Fortran 90 Lehr- und Handbuch,
          BI-Wissenschaftsverlag, 1994.

       Schobert, Oldenburg.
          Programmierung in Fortran 90,
          1991.

       Ueberhuber, C., Meditz, P.
          Software-Entwicklung in Fortran 90,
          Springer Verlag, 1993.
          ISBN 3-211-82450-2

       Wojcieszynski, B, Wojcieszynski, R.
          Fortran 90 Programmieren mit dem neuen Standard,
          Addison-Wesley, 1993.
          ISBN 3-89319-600-5


   * in Dutch,


       Brainerd, W.S., Goldberg Ch.H., Adams J.C.,
          (transl. by J.M. den Haan)
          Fortran 90,
          Academic Service, 1991.
          ISBN 90-6233-722-8


   * in Swedish,


       Blom, K.
          Fortran90 - en introduktion
          Studentlitteratur, Lund, 1994.
          ISN 91-44-47881-X
          URL:  http://www.studli.se/publishing/MBok/M004750/M004788/
                                                         T004788.html

       Einarsson, B., Shokins, Y.
          Fortran 90 for the Fortran 77 programmer
          HTML-book.
          URL:  http://www.nsc.liu.se/~boein/fortran.html


   * in Russian,


       Einarsson, B., Shokins, Y.
          Fortran 90 for the Fortran 77 programmer
          Printed book.
          URL:  http://www.nsc.liu.se/~boein/fortran.html

       Metcalf, Reid
          (translated by P.Gorbounov)
          Fortran 90 Explained.
          Mir Publishers, Moscow, 1995.
          ISBN 5-03-001426-8
          Russian customers: Mr. A.S.Popov, E-mail asp@mir.msk.su
          European residents: Petr.Gorbounov@cern.ch


 * in Japanese


       Metcalf, Reid
          (translated by H.Nisimura, H.Wada, K.Nishimura, M.Takata)
          Fortran 90 Explained,
          Kyoritsu Shuppan Co., Ltd., 1993
          ISSN 0385-6984.


       Articles
       --------


       Appleby, D.,
          FORTRAN First in a six-part series on languages
          that have stood the test of time
          -- BYTE, Sep. 1991, 147-150

       Baker, S.,
          Complying with Fortran90; How does the current crop
          of Fortran90 compilers measure up to the standard?
          -- Dr. Doff's Journal (Jan. 1995) p68-76

       Bernheim, M.,
          Fortran Mode d'emploi - Fortran 90
          -- Intereditions (1991) 163-176

       Brankin, R.W., Gladwell, I.,
          A Fortran 90 Version of RKSUITE: An ODE Initial Value Solver,
          -- Annals of Numerical Mathematics, Vol 1, 1994, in press.

       Buckley, A. G.,
          Conversion to Fortran 90: A Case Study
          -- ACM TOMS Vol20 n 3 Sept.1994 308-353

       Buckley, Albert G.,
          Algorithm 999: A Fortran 90 code for unconstrained
          non linear minimisation
          -- ACM TOMS Vol20 n 3 Sept.1994 354-372
          URL:  ftp://ftp.royalroads.ca/pub/software/bbuckley/

       Chesneaux, J.M.,
          Description d'utilisation du logiciel CADNA_F
          -- MASI 92.32 (1992) Institut Blaise Pascal, Paris

       Corde, P., Girou, D.,
          Fortran 90: la nouvelle norme
          -- Tribunix Dossiers calculateurs, Vol 8. No. 41 (1992) 12-17

       Craig, C., Slishman G.,
          Variants of Matrix Multiplication for Fortran90
          -- SIGNUM Newsletter Vol 29 N 2 Apr. 1994 4-6

       Delves L.M, Schonfelder J.L, Craven P.
          Fortran90; an Overview
          -- Oct.1993 IASC

       Delves M,
          N.A Performance of Fortran90 Compilers
          -- Nov. 1994

       Digital Corporation,
          Evolving from Fortran77 towards Fortran90,
          -- Fall Decus 1993, San Francisco

       Dodson Z.,
          A Fortran90 Tutorial
          -- Nov.1993

       Dongarra, J., Du Croz J., Hammarling S., Wasniewski J., Zemla A.,
          LAPACK90 The Fortran90 Interface for LAPACK,
          -- PARA95, Copenhagen 1995
             Lecture Notes Springer Verlag, to be published.

       Du Croz, Jeremy J.,
          Building Libraries with Fortran 90
          -- Fortran Journal 4/5, Sep./Oct 1992

       Du Croz, J.
          The Nag Fortran90 library
          -- Nagua 14 april 1994 Oxford

       Gehrke, Wilhelm
          Fachwoerterliste Englisch-Deutsch fuer Fortran 90
          -- SPR.F90 2, RRZN, 18 pp., 1995
             URL:  http://www.rrzn.uni-hannover.de/Umdrucke/SPR.F90.2.ps

       Gehrke, Wilhelm
          Fortran 90-Syntax: Eisenbahnschienen-Diagramme
          -- SPR.F90 3, RRZN, 48 pp., 1994
             URL:  http://www.rrzn.uni-hannover.de/Umdrucke/SPR.F90.3.ps

       Gehrke, Wilhelm
          Fachwoerterliste Englisch-Deutsch fuer Fortran 95
          -- SPR.F95 2, RRZN, 19 pp., 1995
             URL:  http://www.rrzn.uni-hannover.de/Umdrucke/SPR.F95.2.ps

       Gehrke, Wilhelm
          Fortran 95-Syntax: Eisenbahnschienen-Diagramme
          -- SPR.F95 3, RRZN, 50 pp., 1995
             URL:  http://www.rrzn.uni-hannover.de/Umdrucke/SPR.F95.3.ps

       Glassy, L.,
          Tiny-Ninety: A subset of F90 for beginning programmers
          -- Fortran Journal 4/3, May/Jun. 1992, 2-6

       Hanson, R.J.,
          A design of high-performance Fortran 90 Libraries
          -- IMSL technical report series No. 9201 (1992)

       Hanson, R.J.,
          Operator and Function Modules with FORTRAN90
          -- VNI Technical Report series No 9305

       Hanson, R.J.,
          Matrix multiplication in Fortran 90 using Strassen's algorithm
          -- Fortran Journal 4/3, May/Jun. 1992, 6-7

       Hennecke, M.,
          A Fortran 90 interface to random Number Generation
          -- Computer Physics Communications, in press
             URL:  http://www.uni-karlsruhe.de/~Michael.Hennecke/
                                              Publications/#CPC95

       Iles, Robert,
          Fortran 90: The First Two Years
          -- Unicom Seminar on Fortran and C in Scientific Computing, 1993.

       Iles, R., Palant, L.,
          Fortran 90: 2 ans deja
          -- Tribunix No. 49 Mai/Juin 1993, 32-37.

       Hann, R.
          Nagware Fortran90 tools
          -- Nagua 14 april 1994 Oxford

       Hill J.M.D
          The high performance Fortran library in Fortran90: sorting
          -- Technical Report LPA7/TR02.9408 The London parallel
             applications center August 1994 (revise 9/1/1995)

       Joubert, A.W
          The high performance Fortran library in Fortran90: prefix
          and suffix scans
          -- Technical Report LPA7/TR01.9408 The London parallel
             applications center August 1994

       Kearfott, R.B
          Algorithm 737: INTLIB: A Portable Fortran77 Interval
          Standard-Function Library
          -- ACM TOMS Vol20 n% 4, Dec. 1994 447-459

       Kearfott, R.B
          A Fortran 90 environment for research and prototyping of
          enclosure algorithms for canstrained and unconstrained
          non linear equations
          -- ACM TOMS Vol 21, 1 , Juin 1995 63-78

       Lahey, T.,
          Fortran 90 is coming !
          -- Programmer's Journal, Mar/Apr 1991.

       Lignelet, P.,
          Fortran -- Les Techniques de l'ingenieur,
          -- H2120, Dec 1993.

       Mc Calpin, John D.
          Optimization of Fortran90 array notation : A Case Study
          -- Internal report College of Marine Studies, Univ. of
             Delaware submitted to "Scientific Programming" Jan. 1995
             URL:  ftp://(perelandra.cms.udel.edu:/models/Papers/f90.ps

       Maine, R.,
          Review of NAG Fortran 90 translator
          -- Fortran Journal 3/6, Nov/dec 1991.

       Marshall,A.C,
          Comparison between Sun, EPC and NAg Fortran 90 Compilers
          -- The University of Liverpool (Dec. 1996).
             URL:  http://www.liv.ac.uk/HPC/FortranCompilerStudyHTML/
                                        FortranCompilerStudyHTML.html

       Marshall,A.C,
          Fortran 90 derived types, User defined operators, Modules
          and Object Oriented Facilities
          -- The University of Liverpool BCS seminar 1994
             (12 Sep. 1992), 30-33

       Metcalf, M.,
          Recent progress in Fortran standardization
          -- Computer Physics Communications 57 (1989) 78-83.

       Metcalf, M.,
          Fortran 90 - A summary
          -- Int. Journal of modern Physics C, Vol. 1,
             Nos. 2&3 (1990) 193-206.

       Metcalf, M.,
          A derived data type for data analysis
          -- Computers in Physics, Nov/Dec 1991, 599-604.

       Metcalf, M.,
          A first encounter with Fortran 90
          -- Fortran Journal 4/1, Jan/Feb 1992, 2-7.

       Metcalf, M.,
          An encounter with F90
          -- Particle World 3/3 (1993), 130-134.

       Metcalf, M.,
          Fortran 90 Tutorial
          -- CERN Computer Newsletter,
             Nos. 206/207/208/209/210/211 (1992-1993).

       Metcalf, M.,
          Using the f90 compiler as a software tool
          -- CERN Computer Newsletter, No. 209 (1992).

       Metcalf, M.,
          Still programming after these years
          -- New Scientist, (12 Sep. 1992), 30-33

       Morgan, S.,
          Fortran90 An outline of the ISO standard
          -- BCS seminar 1994

       Olagnon, M.,
          Experience with NagWare f90
          -- Fortran Journal 4/6, Nov/dec 1992, 2-5.

       Olagnon, M.,
          f90ppr A Fortran90 Pre-processor A Fortran 90 Pretty- printer,
          -- Fortran Journal  Vol 7 n2 Mar/Apr 1995 pp8-14

       de Polignac, Christian,
          Du Fortran VAX au Fortran 90
          -- Decus, Paris, 7 Avril 1993.

       de Polignac, Christian,
          Interfacing a Fortran77 multiple precision package
          using Fortran90
          -- Nagua, Oxford, 14 april 1994.

       Prentice, John K.,
          Fortran 90 benchmark results
          -- Fortran Journal 5/3, May/June 1993.

       Prentice, John K.,
          Performance benchmarks for Fortran90 compilers
          -- Mathematech Vol1 n1 1994, 66-73

       Prentice, John K., Ameko, A.K.,
          Performance benchmarks for selected Fortran90 compilers
          (to appear in Fortran Journal)

       Reid, John,
          The Fortran 90 Standard -- Programming environments for
          high level scientific problem solving,
          -- Gaffney ed., IEEE Trans., North-Holland (1992), 343-348.

       Reid, John,
          Fortran 90, the language for scientific computing in
          the 1990s
          -- Unicom Seminar on Fortran and C in Scientific Computing, 1992

       Reid, John,
          The advantages of Fortran 90
          -- Computing 48, 219-238.

       Reid, John.
          Fortran90: the future
          -- Nagua 14 april 1994 Oxford

       de Roeck, Yann-Herve, Plessix, Rene-Edouard,
          Combining F90 and PVM to construct synthetic seismograms
          by ray-tracing
          -- proc. IEEE Oceans 94.

       Robin, F.,
          Fortran 90 et High Performance Fortran,
          -- Bulletin technique CEA, Oct. 1992, 3-7.

       Sawyer, M.,
          A summary of Fortran 90
          -- EPCC-TN92-04, Univ. of Edinburgh, (1992).

       Schonfelder, J.L.,
          Semantic extension possibilities in the proposed
          new Fortran
          -- Software practice and experience, Vol.19, (1989), 529-551.

       Schonfelder, J.L., Morgan, J.S.,
          Dynamic strings in Fortran 90
          -- Software practice and experience, Vol.20(12), (1990), 1259-1271.

       Schonfelder, J.L.
          High Performance Fortran and Fortran95
          -- University of Liverpool Nov. 1994

       Scott, Kilpatrick and Maley
          The formal specification of abstract data types and their
          implementation in Fortran 90
          -- Computer Physics Communications 84 (1994) 201-225.

       Sipelstein, J.M., Blelloch, G.E.,
          Collection-oriented languages
          -- Proceedings of the IEEE, Vol. 79, No. 4, (1991), 504-530.

       Vignes, Jean,
          Vers un calcul scientifique fiable : l'arithmetique stochastique
          -- La Vie des Sciences, Comptes rendus, serie generale,
             tome 10, 1993, No 2, 81-101.

       Vignes, Jean,
          A stochastic arithmetic for reliable scientific computation
          -- MATCOM 940 - Mathematics and Computers in Simulation
             35 (1993) 233-261.

       Walker, D.W.,
          A Fortran 90 code for magnetohydrodynamics.
          Part I: banded convolution
          -- Oak Ridge National Lab. report TM-12032 (1992).

       Walter, W.,
          Fortran 90: Was bringt der neue Fortran-Standard fuer das
          numerische Programmieren ?
          -- Jahrbuch Ueberblicke Mathematik Vieweg, (1991) 151-174.

       Walter W.V
          Fortran XSC: A portable Fortran90 module library for accurate
          and reliable scientific computing
          -- Computing Supplementum 9, 265-286

       Wampler, K. Dean,
          The Object-Oriented programming Paradigm and Fortran programs
          -- Computers in Physics, Jul/Aug 1990, 385-394.

       Ward, T.
          The world's first Fortran90 compiler.
          -- PROGRAM NOW March 1992, 67-69

       Willhoft, Robert G.,
          Comparison of the functional Power of APL2 and Fortran 90
          -- APL Quote Quad, 1991

       Fortran90 at NAS: Perceptions and plans
          -- RND-93-001
             URL:  http://www.nas.nasa.gov/NAS/TechReports/



       3.6 - Other places for Help on Fortran 90
       -----------------------------------------

       Fortran 90 Tutorials:
          http://wwwcn.cern.ch/asdoc/f90.html

       Programmer's Guide to Fortran 90:
          http://www.fortran.com/fortran/Books/gd.html

       Fortran Market:
          http://www.fortran.com/fortran/market.html

       Karlsruhe University:
          http://www.uni-karlsruhe.de/~Fortran90/

       King's College London:
          http://www.kcl.ac.uk/kis/support/cc/fortran/f90home.html

       Fortran FAQ:
          http://www.cis.ohio-state.edu/hypertext/faq/usenet/
                                         fortran-faq/faq.html

       Fortran90 interface modules for INTLIB interval computations:
          ftp://interval.usl.edu/pub/interval_math/www/

       FTP-able fortran90 Tutorial from ftp.cs.unm.edu:
          ftp://ftp.cs.unm.edu/pub/smith-quetzal/Fortran90_Tutorial/

       Free Software:
          http://www.fortran.com/fortran/free.html

       How to get Fortran 90 Standard documentation:
          http://www.fortran.com/fortran/iso1539.html

       Free Code - At Lahey:
          http://www.lahey.com/other.htm

       Free Compilers/tools List - At Cern:
          http://cuiwww.unige.ch/cgi-bin/freecomp

       Programming Languages research - At Indiana University:
          http://www.cs.indiana.edu/inds/proglang.html

       Other languages - At CMU:
          http://www.cs.cmu.edu/Web/computing.html#language

       - At UNM:
          http://www.arc.unm.edu/workshop/fortran90/f90-7.html

       - The F programming language:
          http://www.imagine1.com/imagine1/



   4.0 - Fortran 90 Benchmarking
   -----------------------------

       An interesting article by John K. Prentice appeared in the
       May/June 93 issue of Fortran Journal.
       He also gave a new one in the Nov/Dec 94 issue.

       I made some tests myself with LAPACK, and got a ratio of 10
       between Sun f77 and Nag f90 2.0 when no source change was performed.
       With an aggressive rewriting, especially using array instructions
       and intrinsics, the ratio gets down to 2, which is also that of a
       f77 [sd]axpy to a C one.

       On actual applications, this ratio seems to be much closer to 1,
       and even sometimes in favor of Fortran 90.
       On Sept. 7th, 1993, John wrote "I think there is in fact beginning
       to be a quite large body of evidence to suggest that most of the
       efficiency fears about F90 are unfounded."

       For Nag f90 on workstations, the effect of the underlying C
       compiler (gcc, vendor, etc...) seems very limited (less than 4%).

       With more recent F90 compilers, performance seems at least as good
       and often better than with the corresponding F77 compiler, for old
       F77 code. For instance, Lahey reports improvement from 8.5 to 14.1
       Mflops with linpack on a pentium between EM/32 and their F90 compiler.



   5.0 Announced, foreseen, and rumours
   ------------------------------------

       F: a carefully crafted subset of Fortran 90, meant for both
          teachers and professional programmers, by Imagine1 Inc.,
          NAG Inc., Fujitsu Limited, and Absoft Corp.
          F will be available on Unix and Linux platforms, the 68k
          or PowerPC Macintosh, and PCs running either Windows 95
          or Windows NT.

       FORTNER Research (formerly Laguage Systems Corp) expects to
          deliver f90 for Macintoshes in 1996.

       Digital Windows NT (Alpha) compiler
          URL:  http://www.digital.com/info/hpc/f90


       MATLAB compatibility with PowerStationFortran 90 (1st quarter 96)



   6.0 Workshops, seminars, conferences
   ------------------------------------

       SEL-HPC:
          the London and South-East centre for High Performance Computing
          URL:  http://www.lpac.ac.uk/SEL-HPC/

       NAG Seminars:
          URL:  http://www.nag.co.uk/other/seminars.html



   7.0 - Developments, related languages
   -------------------------------------

       7.1 - Standard
       --------------

       Work did not stop with the publication of the Fortran 90 standard.
       A new release is scheduled for 1996 (called 95), mainly devoted to
       clarifications, corrections and interpretations. It is currently
       being circulated as a draft for comments. A more important
       revision is scheduled for 2000 (or 2001 ? called F2k though C.Burley's
       F00 is a pleasant alternative).

       Some interim features are to be processed as "technical reports" and
       incorporated in the next major upgrade, now known as "Fortran 2000"
       and planned for release around the year 2000. The features for which
       interim technical reports have been proposed are the following:

          o  Floating-point exception handling
          o  Interoperability with C
          o  Parammeterized derived types and allocatable components

       However, the last of these lacks support in some quarters.

       The ISO working group devoted to the evolution of Fortran is WG5.

          URL:  http://www.etrc.ox.ac.uk/wg5.html

       Inputs are received from the National bodies (X3J3 in the USA).
       Documents related to the work of X3J3 can be found via anonymous
       ftp on ftp.ncsa.uiuc.edu, directory x3j3.


       7.2 - HPF
       ---------

       High Performance Fortran (HPF) is a language for programming
       massively parallel architectures. It lets the user insert
       directives for code and data distribution among the processors
       in the (Fortran 90) code.

          URL:  http://www.erc.msstate.edu/hpff/home.html

       Electronic copies of HPF draft specification are available by
       anonymous FTP from the following sources:

          Machine name            File name
          ---------------------   ----------------------------------------
          titan.cs.rice.edu       public/HPFF/draft/hpf-v10-final.tar
          titan.cs.rice.edu       public/HPFF/draft/hpf-v10-final.tar.Z
          titan.cs.rice.edu       public/HPFF/draft/hpf-v10-final.ps
          titan.cs.rice.edu       public/HPFF/draft/hpf-v10-final.ps.Z
          think.com               public/HPFF/hpf-v10-final.ps.Z
          ftp.gmd.de              hpf-europe/hpf-v10-final.ps.Z
          theory.tc.cornell.edu   pub/hpf-v10-final.ps.Z
          minerva.npac.syr.edu    public/hpf-v10-final.tar.Z


       on-line tutorial from University of Liverpool:
          URL:  http://www.liv.ac.uk/HPC/HTMLFrontPageHPF.html

       course on HPF is freely available from Edinburgh:
          URL:  http://www.epcc.ed.ac.uk/epcc-tec/course-packages/
                                             HPF-Package-form.html

       Other sources of information:

          Karlsruhe University:
             http://www.uni-karlsruhe.de/~HPF/

          Liverpool University:
             http://www.liv.ac.uk/HPC/HPCpage.html

          www.lpac.ac.uk/SEL-HPC:
             http://www.lpac.ac.uk/SEL-HPC/


       7.3 - PVM
       ---------

       Parallel Virtual Machine consists of a library and a run-time
       environment which allow the distribution of a program over a network
       of (even heterogeneous) computers. It works with Fortran 77,
       C and to some extent Fortran 90. One can refer to the article
       by Y-H de Roeck and R-E Plessix, and a set of example wrapper
       routines for the PVM calls is available as:

          URL:  ftp://ftp.ifremer.fr/ifremer/ditigo/fortran90/pvm2f90.tar.gz

       There is a usenet comp.parallel.pvm group, and the FAQ for it
       can be found via anonymous ftp on:

          host:       rtfm.mit.edu
          directory:  /pub/usenet/comp.parallel.pvm


       7.4 - MPI
       ---------

       MPI (Message Passing Interface) is the standard for multicomputer
       and cluster message passing introduced by the Message Passing
       Interface Forum in April 1994.

          URL:  http://www.erc.msstate.edu/mpi/


       7.5 - Parallel Programming
       --------------------------

       An interesting report can be obtained via anonymous ftp on:

         host:      bulldog.wes.army.mil
         directory: pub/
         file:      report.ps.Z

       for a large review of products related to parallel systems
       programming.



   8.0 - Addresses
   ---------------

       3ip,
          104, rue Castagnary,
          F-75015 Paris, France
          tel:  +33 1 48 56 23 33,
          fax:  +33 1 48 56 23 44

       Absoft,
          2781 Bond Street Rochester Hills,
          MI 48309 USA
          URL:    http://www.absoft.com
          tel:    (810) 853-0050 ,
          Fax:    (810) 853-0108
          email:  fortran@absoft.com

       ACE,
          Van Eeghenstraat 100,
          1071 Gl Amsterdam, Netherlands
          URL:  http://www.ace.nl/
          tel:  +31 20 6646416,
          fax:  +31 20 6750389

       AERO, Mr. Berthon,
          3 av. de l'opera. F-75001 Paris,
          France
          tel:  +33 1 44 55 30 80,
          fax:  +33 1 40 15 95 54

       AFNOR,
          Tour Europe,
          Cedex 7,
          F-92049 Paris la Defense,
          France
          tel:  +33 1 42 91 55 55

       Apogee Software Inc.,
          1901 S.Bascom Ave.,
          Suite 325,
          Campbell,
          CA 95008-2207, USA
          URL:    http://www.apogee.com/
          tel:    (408) 369-9001,
          fax:    (408) 369-9018,
          email:  info@apogee.com

       Applied Parallel Research, Inc.,
          550 Main St.,
          Placerville,
          CA 95667
          URL:    http://ftp.netcom.com/pub/forge/home.html
          tel:    (916) 621-1600,
          fax:    (916) 621-0593,
          email:  support@apri.com

       CETech, Inc.,
          8196 SW Hall Blvd.,
          Ste. 304, Beaverton,
          Oregon 97008, USA.
          tel:    (503) 644-6106,
          fax:    (503) 643-8425,
          email:  cetech@teleport.com

       Cray Research,Inc.,
          655 Lone Oak Drive,
          Eagan, MN  55121
          URL:  http://www.cray.com/

       CTS,
          Prinz-Otto Str. 7c,
          D-85521 Ottobrunn,
          Germany
          tel:  +49 89 6083758,
          fax:  +49 89 6083758

       DEC (Digital Equipment Corporation)
          URL:    http://www.digital.com/info.html
          email:  f90@digital.com

          DEC Fortran 90 home page:
             http://www.digital.com/info/hpc/f90

       EPC,
          17 Alva St. Edinburgh,
          EH2 4PH, United Kingdom
          URL:    http://www.epc.co.uk/
          tel:    +44-31-225-6262,
          fax:    +44-31-225-6644,
          email:  support@epc.ed.ac.uk

       EPC,
          20 Victor Square,
          Scotts Valley,
          California 95066
          tel:    (408) 438-1851,
          fax:    (408) 438-3510,
          email:  info@epc.com

       Fortran Journal,
          P.O. Box 4201,
          Fullerton,
          CA 92634, USA
          fax:  (714) 441-2022

       Fujitsu Open Systems Solutions, Inc.,
          3055 Orchard Drive,
          San Jose,
          CA 95134 USA
          URL:    http://www.fortran.com/fortran/Fujitsu/fuji.html
          tel:    (408) 456-7809,
          fax:    (408) 456-7050,
          email:  info@ossi.com

       Garnatz et Grovender Inc.,
          5301 26th Avenue South,
          Mineapolis MN 55417-1923 USA
          tel:    (612) 722-3094,
          email:  gginc@winternet.com

       HP
          URL:  http://www.hp.com/go/workstations

       IBM
          URL:  http://www.torolab.ibm.com:80/ap/fortran/xlfortran/

       ICHOR,
          27 rue Linne,
          F-75005 Paris,
          France
          tel:  +33 1 43 37 02 02

       IDRIS,
          B.P. 167,
          F-91403 Orsay Cedex,
          France

       Imagine1,
          11930 Menaul Blvd. NE,
          Suite #106, Albuquerque,
          NM 87112, USA
          URL:    http://www.imagine1.com/imagine1
          fax:    (505) 323-1759,
          tel:    (505) 323-1758,
          email:  info@imagine1.com

       ISO,
          1 rue de Varembe,
          Case postale 56,
          CH-1211 Geneve 20,
          Switzerland
          fax:  +41 22 734 10 79

       Interactive Software Services Ltd.,
          25 St Michaels Close,
          Penkridge,
          Stafford ST19 5AD, UK
          tel:    +44 1785 715588,
          fax:    +44 1785 714913,
          email:  support@issltd.demon.co.uk

       IT Independent Training Limited,
          113 Liscombe,
          Birch Hill, Bracknell,
          Berkshire, RG12 7DE, UK
          tel:  +44 344 860172,
          fax:  +44 344 867992

       KAI (Kuck & Associates),
          Champaign, IL USA
          tel:    (217) 356-2288,
          fax:    (217) 356-5199,
          email:  katy@kai.com

       Lahey Computer Systems, Inc.,
          865 Tahoe Blvd.,
          P.O. Box 6091,
          Incline Village,
          NV 89450, USA
          URL:    http://www.lahey.com/
          tel:    (702) 831-2500,
          fax:    (702) 831-8123,
          email:  sales@lahey.com

       Microsoft
          URL:  http://www.microsoft.com/fortran

       Microway,
          Research Park, Box 79,
          Kingston, MA 02364, USA
          tel:    (508) 746-7341,
          fax:    (508) 746-4678,
          email:  nina@microway.com

       NA Software Ltd,
          Roscoe House,
          62 Roscoe St.,
          Liverpool L1 9DW, UK
          tel:    +44 51 7094738,
          fax:    +44 51 7095645,
          email:  f90doc@nasoftwr.demon.co.uk

       NAG Ltd.,
          Wilkinson House,
          Jordan Hill Road,
          Oxford, OX2 8DR, UK
          URL:    http://www.nag.co.uk/
          tel:    +44 1865 311744,
          fax:    +44 1865 311755,
          email:  infodesk@nag.co.uk

       NAG Inc.,
          1400 Opus Place,
          Suite 200, Downers Grove,
          IL 60515-5702, USA
          tel:    (708) 971-2345,
          fax:    (708) 971-2346,
          email:  infodesk@nag.com

       NAG GmbH.,
          Schleissheimerstr. 5,
          D-85748 Garching, Germany
          tel:  +49 89 3207395,
          fax:  +49 89 3207396

       NAG Office,
          Espace III,
          62 Boulevard Frederic Arnaud,
          09200 Saint Girons
          (Toulouse, France)

       NAG Users Association,
          PO Box 426,
          Oxford, OX2 8SD, UK
          tel:    +44 1865 311102,
          fax:    +44 1865 310139,
          email:  nagua@nag.co.uk

       Pacific-Sierra Research Corp.,
          2901 28th Street,
          Santa Monica, CA 90405
          URL:    http://www.psrv.com
          tel:    (310) 314-2300,
          fax:    (310) 314-2323,
          email:  info@psrv.com

       ParaSoft Corporation,
          2500 E. Foothill Blvd,
          Pasadena, CA 91107, USA
          tel:    (818) 792-9941,
          email:  f90-info@parasoft.com

       PGI, The Portland Group,
          9150 S.W Pioneer Ct.,
          Suite H Wilsonville,
          OR 97070 ,USA
          URL:    http://www.pgroup.com/
          tel:    (503) 682-2806,
          fax:    (503) 682-2637
          email:  sales@pgroup.com

       Quetzal Computational Associates,
          3200 Carlisle N.E.,
          Albuquerque,
          NM 87110-1664, USA
          tel:    (505) 889-4543,
          fax:    (505) 889-4598,
          email:  quetzal@aip.org

       Salford Software,
          Adelphi House, Adelphi Street,
          Salford M3 6EN, UK
          tel:    +44 161 8342148,
          fax:    +44 161 8342454,
          email:  sales@salfsoft.demon.co.uk

       S.I. editions,
          9 av. Prince Hereditaire Albert,
          MC-98000, Monaco
          tel:  +33 92 05 35 51,
          fax:  +33 92 05 35 04

       Simulog,
          1 rue James Joule,
          F-78286 Guyancourt Cedex, France
          tel:    +33 1 30 12 27 00,
          fax:    +33 1 30 12 27 27,
          email:  plestan@simulog.fr  (Mr. E. Plestan)

       Spackman & Hendrickson, Inc.,
          13708 Krestwood Drive,
          Burnsville,
          MN 55337,  USA
          tel:  (612) 892-5847,
          fax:  (612) 892-5844

       Sun Micro Systems
          URL:  http://www.sun.com/

       Unicom Seminars Ltd.,
          Brunel Science Park,
          Cleveland Road, Uxbridge,
          Middlesex, UB8 3PH, UK
          URL:    http://www.demon.co.uk/unicom/
          tel:    +44 895 256484,
          fax:    +44 895 813095,
          email:  unicom@unicom.demon.co.uk

       Unicomp, Inc.,
          1874 San Bernardino Ave NE,
          Albuquerque, NM 87122, USA
          tel:    (505) 275-0800,
          fax:    (505) 856-1501,
          email:  walt@fortran.com

       Visual Numerics,
          URL:    http://www.vni.com/
          email:  mktg@houston.vni.com


       I am always pleased to receive informations.
       Thanks to all those who sent some to me, and that I can not cite
       all because I lost some of their names and addresses :-)

       Michel


       | Michel OLAGNON            | email : Michel.Olagnon@ifremer.fr  |
       | Centre de Brest - B.P. 70 | phone : +33 2 98 22 41 44          |
       | F-29280 PLOUZANE - FRANCE | fax   : +33 2 98 22 41 35          |
       | WWW: http://www.ifremer.fr/ditigo/molagnon/molagnon.html       |

       IFREMER: Institut Francais de Recherches pour l'Exploitation de la Mer

          URL:  http://www.ifremer.fr

       De'partement Ge'nie Oce'anique

          URL:  http://www.ifremer.fr/ditigo/ditigo.uk.html

       Cellule Oce'ano-Me'te'o

          URL:  http://www.ifremer.fr/ditigo/com/com.html


   __________________________________________________________________________
                                       


1.3.2) Fortran Market

       ------------------------------------------
       ~Subject: (SC22WG5.609) Fortran Market/WWW
       ------------------------------------------

       I hope all of you will be pleased to learn that the Fortran Market
       has established itself on the World Wide Web.  Our goal is nothing
       short of providing one place to find all information, products,
       and services related to Fortran.  The URLs are:

          http://www.fortran.com/fortran/market.html
          http://www.fortran.com/walt/fortran

       The Market is under construction (and probably always will be),
       but there is already some free software available (just some
       simple, but perhaps useful, things so far).  There are pointers
       to other locations containing relevant information, so you now
       need to remember only one place to find it all.  Much more
       information, particularly about products and servies will be
       available in the near future, but I thought you might want to
       have a Sneak Preview of what things will look like.

       Come visit the Market and let me know what you think of it.

          Thanks. <walt>



  ;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;



2.1) Compilers and preprocessors


2.1.1) Where can I get a free (FORTRAN 77) compiler?

       There are few such in wide distribution:

          o  f2c + any C compiler
          o  f2c combined with djgpp
          o  A combination of (f2cx + gcc + djgpp extender)
          o  GNU's g77
          o  BC-F77


;; One such is f2c:

       -----------------------------------------
       ~From: mwm@a.gp.cs.cmu.edu (Mark Maimone)
       -----------------------------------------

       Since there have been several requests for a Fortran to C translator
       in the past week, I'm reposting the announcement about f2c.
       The short answer is you can get f2c by anonymous ftp
       from:

          host:       netlib.att.com
          directory:  dist/f2c.

       -----------------------------------------------------------------

       Source for f2c, a Fortran 77 to C translator jointly developed by
       folks from Bell Labs, Bellcore, and Carnegie Mellon, is now freely
       available.

       F2c was derived from the original UNIX operating system's f77(1),
       and the generated C follows f77's calling conventions; on some
       machines, the resulting object files are interchangeable with
       (and behave indistinguishably from) objects compiled by f77.

       The main "advantage" of f2c is that it converts ANSI standard
       Fortran 77 into C without manual intervention, at least when
       invoked by a suitable script or makefile (that may need to
       exercise an f2c option to ensure that COMMON blocks are defined
       just once).

       The main "problems" are that f2c does no code restructuring
       (e.g., gotos are preserved) and that Fortran I/O gets converted
       into a bunch of calls; thus the translated C code doesn't look
       too pretty, and in general one would need to maintain the Fortran
       rather than its translation into C.  [F2c is not meant to displace
       the services of commercial vendors whose business is to convert
       Fortran into maintainable C.]

       There is a plethora of options, many of which exist to support
       different compilation environments for the translated C (e.g.,
       ANSI C or C++ compatibility, different type sizes, separate files
       for COMMON blocks to appease "smart" linkers).

       So far f2c (and f2c-generated source) has compiled successfully
       on many machines: Sun, Vax, IBMRT, Apollo, SGI, MIPS, and Cray
       to name a few.

       F2c has been under test by the net community for over a year and
       has been verified on the NBS tests, several large math libraries,
       floating point tests, even code for laying cable on the ocean floor!

       To find out about f2c, send the following E-mail message
       to netlib (netlib@research.att.com  or  research!netlib):

          send index from f2c

       Your message will be answered automatically (by a program --
       see CACM vol.  30 #5 (May, 1987), pp. 403-407).

       You will receive a reply explaining how to automatically acquire f2c
       source  (about 600K), f2c library source (130K), and supporting info
       (man page, etc).  Or you can anonymous-FTP to:

          research.att.com

       and look in directory dist/f2c at these files:

          all.Z --               250K compressed shar file for f2c
          f2c.ps.Z --            24 page tech report describing f2c
          index --               general info about files
          libf77.Z, libi77.Z --  compressed shar files for libraries


       ******************************
                DISCLAIMER
       ******************************
        Careful! Anything free comes with no guarantee.

       ---
       Mark Maimone                            phone: (412) 268 - 7698
       Carnegie Mellon Computer Science        email: mwm@cs.cmu.edu
                                                      cmcspt!mwm@cs.cmu.edu

       Notes:  f2c accepts only fairly vanilla FORTRAN; vendor supplied
               f77's usually produce better quality code, and accept a
               wider variety of codes.



   More about f2c from Judah Milgram
   ---------------------------------

       I recently asked about running f2c with djgpp. Turns out to be
       easy and together they make a good Fortran compiler for PC's.
       Here's a summary.

       I started with f2c dated Nov. 1994 (netlib.att.com in netlib/f2c).
       djgpp was v. 1.12 (omnigate.clarkson.edu in pub/msdos/djgpp.)

       Use the pre-compiled msdos f2c executable that comes with the
       f2c release. Compile the libraries with djgpp, making the changes
       listed below. They aren't necessarily the most sensible changes,
       but they worked for me. Write if you have a better idea.

       Thanks to all net people who helped, especially Dr. James Lupo.

          Judah Milgram
          milgram@glue.umd.edu
       _______________________________________________


          libf77/makefile:

             change:       CC = cc
             to:           CC = gcc
             comment out:  ld -r -x -o $*.xxx $*.o
                           mv $*.xxx $*.o

          libf77/s_paus.c:

             change:       extern int getpid(void), isatty(int), pause(void);
             to:           extern int getpid(void), isatty(int);
                           #ifndef _djgpp_std_h
                           extern int pause(void);
                           #endif

          libi77/makefile:

             change:       CC = cc
             to:           CC = gcc
             comment out:  ld -r -x -o $*.xxx $*.o
                           mv $*.xxx $*.o

          libi77/fio.h:

             add to top of file:  #ifdef abs
                                  #undef abs
                                  #endif

          libi77/rawio.h:

             comment out entire block:  #ifdef MSDOS
                                        #include "io.h"
                                        #define close _close
                                        #define creat _creat
                                        #define open _open
                                        #define
                                        read _read
                                        #define write _write
                                        #endif

          Easiest way to build libf2c.a is to go into
          the f2c/ directory and do:

             ar r libf2c.a libf77/*.o libi77/*.o
             ranlib libf2c.a

          (If you do it this way you can delete libf77/libf77.a
           and libi77/libi77.a)

          Then copy libf2c.a into djgpp/lib and copy f2c.h into djgpp/include
          And remember to run the executable with 'go32 foo'.
          Or, do 'coff2exe foo' to produce a .exe file which
          you can run in the usual manner.


       ---------------------------------------------
       ~From: Greg Lindahl <gl8f@fermi.clas.virginia.edu>
       ---------------------------------------------

       f2c is quite free.



 A ready to use package (F2CX + GCC + DJGPP) from Clive Page:

       I have packaged up a free Fortran77 system for MS-DOS into two
       files which are each just under 1.4 MB (to fit on 2 floppy disks).

       This isn't actually a compiler but relies on the F2CX translator
       to convert Fortran77 into C, and then GNU's GCC compiler plus the
       DOS-extender of DJGPP to get a flat 32-bit address space on MS-DOS.

       This sounds awkward to use, but works surprisingly well on most
       Fortran code that I have used.  Warning: this is free software,
       no warranties at all, but it works for me and some of my colleagues
       also say it works for them.

       The files are available by anonymous FTP from:

          host:       ftp.star.le.ac.uk in
          directory:  pub/fortran
          files:
                      ff77.tex        Instructions for installation and use,
                                      Latex format (22k)
                      ff77.ps         Ditto, but in Postscript (99k)
                      ff77.000        First binary file (1.4 MB)
                      ff77.001        Second binary file (1.1 MB)
                      tar.exe         DOS version of Unix TAR, needed to
                                      extract s/w (52k)

       Transfer the ff77.tex (or .ps) file in ASCII mode, the others
       need BINARY mode.

       In the same directory you will also find an electronic copy of
       a Fortran77 book which I wrote some years ago.  It's available
       in Latex and Postscript form in compressed (gzip) files

           prof77.tex.gz  (113 kbytes)
           prof77.ps.gz   (224 kbytes)

       Enjoy.



;; gnu g77:

       -----------------------------------------------------
       ~From: zrzm0111@helpdesk.rus.uni-stuttgart.de (MUFTI)
       -----------------------------------------------------

       The FSF has a f77 front end integrated with the gcc back end.

       "A mailing list exists for those interested in the Fortran
       front end for GCC. To subscribe, ask:

          info-gnu-fortran-request@prep.ai.mit.edu

       Or try:

          finger -l fortran@gate.gnu.ai.mit.edu

       There is no FSF project to do a f90 front end. The author
       of the g77 front end is willing, if anyone will fund it.


       --------------------------------------------------------
       ~From Bill Thorson <thorson@typhoon.atmos.colostate.edu>
       --------------------------------------------------------

       GNU Fortran (g77) Copyright (C) 1995 Free Software Foundation, Inc.

       GNU Fortran (g77) Version 0.5.13 is now available to the
       public for beta testing in the usual GNU locations.
       The distribution is named:

          g77-*.tar.gz.  Where the '*' is the current version number.
          g77 requires that you also have a recent distribution of gcc.
          This compiler currently builds and installs it's own version
          of the f2c libraries (libf2c.a).

       See g77 documentation for list of features or bugs.

       Most GNU software is packed using the GNU `gzip' compression
       program.  Source code is available on most sites distributing
       GNU software.

       For information on how to order GNU software on tape, floppy
       or cd-rom, or printed GNU manuals, check the file etc/ORDERS
       in the GNU Emacs distribution or in GNUinfo/ORDERS on prep,
       or e-mail a request to:

          gnu@prep.ai.mit.edu


;; gnu update on g77:

       --------------------------------------------------
       Sender: Michael.Taeschner@Student.Uni-Magdeburg.DE
       --------------------------------------------------

       Hi,

       since I read question 2.1.1 at least once a week in this newsgroup,
       I  would like to refer the asking (usually students, who need
       fortran for some  kind of project, but do not want to spend a
       lot of money) to your FAQ  like others do.

       Unfortunately I think that the info in this section is somewhat
       rather old. I would encourage you to make additions regarding
       the availibility of g77:

          1. g77 is now at version 0.5.18, it should be used with
             gcc-2.7.2, because of some improvements in both.
             It works quite stable and allows (in difference to f2c/gcc)
             the debugging at source code level (with gdb, newer versions).

          2. There are binaries in many linux-distributions,
             so you are not required to compile it yourself
             (which is not too difficult, but some work)

          3. Michael Holzapfel provided OS/2 binaries using the
             emx-port of gcc. He wrote, that he will try to keep
             them up-to-date for the next two years.
             These can be found for instance at:

                ftp.leo.org

             but many other os/2-mirrors carry them too,
             one might use archie.

             Because most students search a compiler for MS-DOS,
             I want to emphasize, that these are running fine
             under DOS and take advantage of all available memory.
             With the additional rsx-package they run also
             with win3.1, win/nt and win95.

          4. I tried the recommended  bcf for DOS some time ago and
             was not able to run any fortran code. (maybe I'm stupid)
             The system seems to be mainly for teaching fortran and
             is rather limited.

             Anyone who wants to compile and run real applications
             should g77 give a try, it's worth every cent.


BC-F77:

       ------------------------------------------
       ~from: Kurt Jaeger pi@rus.uni-stuttgart.de
       ------------------------------------------

       Someone asked for a cheap MS-DOS Fortran compiler for students.
       The bcf77 by Andreas Koesterli has a free student version.
       The student version may not be used in a comercial enviroment
       or to solve commerical problems.

       It's a version that writes a non-standard object format
       and requires 640KB.  If all input is in UPPERCASE, it
       supports the full Fortran 77 standard.

       The site is:  ftp.uni-stuttgart.de

       the compiler can be found in:

          /pub/systems/pc/lang/fortran/compiler/bcf77.zip

       It can be accessed via:  ftpmail@ftp.uni-stuttgart.de

       for those of you without ftp.


       -----------------------------------------
       ~From: barbee@noir.llnl.gov (Troy Barbee)
       -----------------------------------------

       In article <1991Dec11.160531@IASTATE.EDU>, cfrandal@IASTATE.EDU
       (Charles F Randall) writes:

       |> Note that the .txt file for this NOT in English:
       |> |> BC-FORTRAN77 Version.b besteht aus Compiler, Linker,
       |> Modulbibliothek und einem residenten Laufzeitsystem, das
       |> u.a. einen einfachen Debugger enthaelt. Diese Version
       |> laeuft auf einem MS-DOS Rechner mit 640kB RAM.  Eine
       |> Festplatte ist nicht erforderlich. Hiermit soll in
       |> einfacher Weise ein Compiler fuer Programmierkurse
       |> zur Verfuegung stehen. Dem kommt entgegen, dass
       |> entsprechende Compiler fuer ATARI ST und AMIGA existieren.
       |> |> Anfragen nach Zusendung einer anderen oder neueren Version
       |> werde ich nur noch beantworten, wenn DM 20.- (Schein oder
       |> Scheck) Aufwandsentschaedigung (Diskette, Umschlag, Porto
       |> und Zeit) beigefuegt sind. Ich versende ausschliesslich
       |> 3 1/2 Zoll Disketten.
       |> |> Anybody willing to translate?

       Here's a quick and dirty translation (i.e., I didn't look in my
       dictionary, so the sentences in [] are just rough translations)

          BC-FORTRAN77 Version b consists of a compiler, linker,
          module library, and a resident runtime system that contains
          (among other things) a simple debugger.
          This version runs on a MS-DOS computer with 640KB RAM.
          A hard disk is not required.
          [The intent is to provide a compiler for programming
          courses in a simple manner. Similar compilers exist
          for the ATARI ST and the AMIGA.]

       Requests for another or a newer version will only be answered
       if they are accompanied by DM 20.- (check or cash) to defray
       costs (diskette, envelope, postage, and time).
       I can only send 3 1/2 inch diskettes.


       ----------------------------------------
       ~From: pmh2962@zeus.tamu.edu (Pat Hayes)
       ----------------------------------------

       "BC-FORTRAN 1.3b, is a FORTRAN compiler from Germany.
       The documentation is in German. Sample source code is included.
       The compiler generates big, inefficient EXE programs and is
       offered only because there are no other pd/shareware
       FORTRAN compilers available.
       700K of disk space is required."


       ------------------------------------------------------
       ~From: PVT Joe Snuffy <DOYLECM@ROSEVC.Rose-Hulman.Edu>
       ------------------------------------------------------

       I am sort of asking for your help here.

       I translated the documentation for BC-F77 and am willing
       to make it available to people.  However, my newsreader
       will not let me post with distribution wider than our local
       site (or at least, that appears to be what is going on).

       Could you do me a favor and post the text that follows?
       You might also tell those others who write to you that
       this translation is available.

          Chris Doyle
          DoyleCM@RoseVC.Rose-Hulman.Edu


       Stuff to be posted starts below this line.  Adjust
       header/newsgroup/etc as appropriate.  Thanks!


          ------------------------------------
          ~From: doylecm@HYDRA.ROSE-HULMAN.EDU
          ------------------------------------

          For those people who FTP this thing and want to be able to
          read the documentation, I have translated the README file
          into English and will let you have a copy of the translation
          upon request. Translation is about 400 lines long.

          BCF77 (FORTRAN 77 compiler, written by Andre Koestli) distribution.
          This compiler/linker/run-time module and supporting files are
          available via anonymous FTP from:

             host:       uni-stuttgart.de
             directory:  /soft/pc/lang/fortran/compiler/
             file:       bcf77.zip


       -------------------------------------------------------------
       ~From: alan@dmsmelb.mel.dms.CSIRO.AU Wed Jan 26 12:27:49 1994
       -------------------------------------------------------------

       BCF is available by ftp from many places.
       For instance, it is in the directory  fortran  on simtel (see q3).
       I did  `archie bcf'  and found it is also in directory:

          host:       src.doc.ic.ac.uk
          directory:  /usenet/comp.archives/languages/fortran

       ...  There have been many complaints about bcf - but it is free.
       I recommend Lahey's Personal Fortran PF77L to those who have been
       disappointed with bcf.  I believe it costs US$99.


   __________________________________________________________________________
                                       


2.1.2) What is the best (FORTRAN 77) compiler for a PC?

       There are many products, some are quite good. Few are free.
       f2c and gcc can be had for the PC environment.

       Popular ones are:

          Lahey (very fast compilation; excellent reputation for support)

          Watcom (touted for good optimization)

          MicroWay (support for odd floating point units)

          LPI (multi-platform support)

          MicroSoft (various good hooks into windows and such)

          Absoft (multi-platform support)

       It is beyond the scope of a faq to provide a commercial endorsement.


   __________________________________________________________________________
                                       


2.1.3) What is the best Fortran for...

       Such recommendations are, at best, personal opinions.
       I've <khb> tracked some of the discussions and it
       would appear that:

          a) For the mac, Language Systems

             Language Systems Corp.
             100 Carpenter Drive
             Sterling, VA 20164

             tel:  800-252-6479 (inside US and Canada)
                   703-478-0181
             fax:  703-689-9593
             BBS:  703-709-0134

             langsys         (Applelink)
             langsys         (America Online)
             langsys@aol.com (Internet)

          b) For the PC it is harder. Many like Lahey

             Lahey Computer Systems, Inc.
             865 Tahoe Blvd.
             P.O. Box 6091
             Incline Village, Nevada 89450

             Phones: (800) 548-4778
                     (702) 831-2500
             Fax:    (702) 831-8123
             BBS:    (702) 831-8023.
             UUNET: Sales        sales@lahey.com
                    Tech support support@lahey.com

             Good code generation, good diagnostics, fast compilation,
             and good support are often quoted as reasons why folks
             liked LCS.


   __________________________________________________________________________
                                       


2.1.4) What Fortran 90/95 compilers/translators (math libs) are available?

   A fortran 95 compiler
   ---------------------

       ------------------------------------------------
       ~From: David Vallance <DMV@salford-software.com>
       ------------------------------------------------

       (16 December 1996)

       FULL F95 COMPILER AVAILABLE FROM SALFORD SOFTWARE LTD
       =====================================================

       Salford Software Ltd announces FTN95, a full Fortran 95
       compliant compiler for Extended DOS, Windows 3.1 and
       Win32 (NT and 95).  The compiler is delivered as a bundle
       comprising a Win32 Edition and an Extended DOS/Windows 3.1
       edition.  FTN95 compilers are supplied with fully-featured
       IDE, debugger, comprehensive compiler library (which
       includes graphics, operating system access, low-level file
       management, bit-manipulation, sorting, etc.), built-in 32
       bit assembler, linker and Salford ClearWin+ (Salford's
       Windows GUI development library and tools).  Salford FTN95
       will ship in Q1 1997.

       Selected Salford-specific features
       ==================================

       o  Full support for REAL*10, COMPLEX*20

       o  Compatibility with Salford FTN77:

          - Inline Mnemonic Assembler using CODE ... EDOC.

          - Supports all 'deleted' Fortran 95 features (e.g.  REAL
            DO-loop indices).

       Shipping:
       ========

       Beta: early January 1997

       First customer ship: Q1 1997

       Beta Testers Wanted
       ===================

       Salford FTN95 will ship in Q1 1997 and will be available to
       selected users for beta test from early January 1997.

       If you would like to apply for a beta copy of FTN95 please
       contact Ivan Lucas at:

          ftn95beta@salford-software.com

       stating your affiliation (e.g.   WG5 member), full mailing
       address and whether you would like to try either or both of
       the Win32 or Extended DOS editions.  The beta editions are
       supplied on (a small number of) 3.5" diskettes.

       FTN95 is a registered trademark of Salford Software Ltd.

          David M Vallance

       Salford Software Ltd      Tel: +44 (0) 161 834 2454
       Adelphi House             Fax: +44 (0) 161 834 2148
       Adelphi Street            WWW: http://www.salford.ac.uk/ssl/ss.html
       Salford, M3  6EN
       UK


   Fortran 90 compilers
   --------------------

       Apogee
          compiler for SPARC architectures (info@apogee.com).
          Used on the Meiko CS-2HA.

       APR
          Useful tools, like FORGE90 are available (forge@netcom.com).
          A source form convertor, convert.f90, is obtainable by
          ftp from:

             host:       jkr.cc.rl.ac.uk
             directory:  /pub/MandR.

       Cray Research
          has a native compiler that is being marketed by them
          and Visual Numerics for workstations, starting with
          Suns (solaris 2.3+) (craysoft@cray.com).
          Absoft will market a PC version (486,Pentium and Macintosh PowerPC)
          (fortran@absoft.com).

       DEC
          has been shipping a native compiler, including HPF,
          from June 1994.  It is for OSF/1 AXP, with probably 
          Windows NT AXP following. It has no plans for VAX systems.

       EPC
          Native compilers for Sun, RS/6000, SGI, MIPS and, soon,
          x86 are available (info@epc.com or support@epc.ed.ac.uk).

       Fujitsu
          is marketing a native Fortran 90 Workbench for
          Solaris 1.1 and 2.x.
          Contact Unicomp (walt@fortran.com) or Fujitsu (info@ossi.com).

          Fujitsu Fortran is fully compliant with the Fortran 90
             (ISO/IEC = 1539:1991), the FORTRAN 77 (ANSI X3.9-1978),
             and the FORTRAN 66 (ANSI X3.9-1966) standards.
             Language extensions include support for Sun, Cray, VAX, and IBM.
             Fujitsu Fortran delivers faster performing FORTRAN 77 code
             while improving developer productivity of your Fortran 90 code.
             <tay@fsc.fujitsu.com>

          SSL2 is a complete library of optimized mathematical routines.
             Initially created for supercomputers and mainframes,
             Fujitsu SSL2 delivers maximum performance to your workstation.
             Through joint development with universities, these numerical
             algorithms provide the accuracy and reliability you require
             in your applications. For additional information please see:
             http://www.adtools.com/lpg/fortranhp.htm
             <Todd, Office: tay@adtools.com, Home todd@yancey.com>

       HP
          announced on Nov. 11, 1996 its full ISO Fortran 90 compiler,
          featuring:

             o  Front End by Edinburgh Portable Compilers (EPC)

             o  Industry standard language extensions: Cray pointers,
                INTEGER*8, REAL*16 and DEC structures.

             o  Scalability - The same compiler runs on all
                high-performance HP computers.

             o  Binary compatability with f77 - object modules compiled
                with f77 and f90 can be mixed (same I/O libraries).

             o  Supports HP MPI (Message Passing Interface) for parallel
                application development. Support for HPF through Portland
                Group HPF package

             o  EUC and multibyte character support.

          Comes with a preprocessor, graphical-task-oriented debugger
          that can debug optimized code (except at the highest level),
          performance analyzer and incremental linker (links only
          modified modules).

          User licenses are priced at $1,495 per user license.
          The HP exemplar server user license is priced at $3,000.

          Additional information on HP Fortran 90 is available at:

             http://www.hp.com/go/hpfortran


       IBM
          has been shipping its optimizing, native compiler for the
          RS/6000, xlf Version 3, as of 31 December, 1993.

       IMSL (now Visual Numerics, mktg@houston.vni.com)
          are beginning to offer f90 versions of their maths libraries
          that take full advantage of the language's library building
          capabilities.

       Lahey
          has been shipping a native LF90 compiler for DOS
          since 29 August, 1994 (sales@lahey.com).
          It is particularly well optimized on the Pentium.

       Microsoft
          is working on a compiler, release date unknown, for
          Windows NT 3.5 and Windows 95 (Chicago) (fortran@microsoft.com).

       Microway
          NDP Fortran 90 for 386/486, Pentium and 860 is available
          (tel. (508) 746-7341).

       NAG
          A compiler is available for most unix platforms, VMS and PCs
          (including Linux) from NAG (infodesk@nag.com or infodesk@nag.co.uk).
          This was the first f90 compiler, released in 1991.
          The current version is 2.1.
          For more information see:  http://www.nag.co.uk/1h/nagware.html

          NAG are beginning to offer f90 versions of their maths libraries
          that take full advantage of the language's library building
          capabilities.
          NAG contact info: NAG FL90 from  infodesk@nag.com,
                                           infodesk@nag.co.uk
                       and  http://www.nag.co.uk/1h/numeric.

       NA Software
          supplies Fortran 90 Plus on 386/486, SPARC and T800
          and T9000 transputers (marketing@nasoftwr.demon.co.uk).
          They also supply a F77 to f90 convertor, LOFT90, and HPF.

       PSR
          VAST/f90 is a complete f90 compiler, including a vectorizer,
          for unix, VMS and Convex (info@psrv.com).
          PSR also supplies VAST/77to90 to convert FORTRAN 77 programs
          into Fortran 90 syntax.

       ParaSoft
          A compiler is available (f90-info@parasoft.com).

       PGI
          has released a subset Fortran 90/HPF compiler,
          in particular for SGI (sales@pgroup.com).

       Salford Software
          A PC version of the NAG compiler is also available
          from Salford Software (ppatel@cix.compulink.co.uk).
          A Windows NT version is planned.

       SofTech
          has a licence to sell its own versions of
          DEC's HPF/f90 compiler.

       Stern Computing Systems
          offers CF90, a Cray-compatible compiler for use
          on DEC OSF/1 platforms (pipeline@acri.fr).

       Sun (to be precise, the Developer Products group of SunSoft)
          has announced a native f90 compiler. It is available as the
          "Performance Workshop for Fortran 90" and includes the first
          release of the SPARCompiler Fortran 90 that is based on the
          CF90 product from Cray.
          Also included is SunSoft Performance Library (tuned versions
          of BLAS[123], LAPACK, FFTPACK, VFFTPACK, licensed from DSS),
          and the usual programming environment addons (debugger,
          performance analyzer, group source code management etc.).
          f77 and C compilers are also provided in the Performance Workshop.
          30 day free demos are available. For more information see:
             http://www.sun.com/sunsoft/Products/Developer-products.

       Linux compilers and related information:
          http://marie.mit.edu/~templon/fortran.html

       Visual Analyzer
          Visual Analyzer is a set of development tools to graphically
          display source analysis of your Fortran and C code.
          The Visual Analyzer includes the Source Analyzer and
          Node Coverage tools to make code migration, performance
          tuning and code maintenance simple.
          And, Visual Analyzer can be used with other Fortran and
          C compilers available for the Microsoft Windows 95/NT
          and SPARC environment.

       Visual Numerics
          see IMSL


   __________________________________________________________________________
                                       


2.1.5) Tell me about Parallel Fortran dialects, what are they,etc.

       -------------------------------------
       ~From: lfm@pgroup.com (Larry Meadows)
       -------------------------------------

       spencer@glint.mcc.com (Steve Spencer) writes:

       >We are trying to decide what parallel FORTRAN environment
       >to port to a MIMD multiprocessor that we are building
       >for ARPA. We are looking for information on the follwing
       >environments:
       >       FORTRAN90
       >        HPF (High Performance FORTRAN from Rice U. I think)
       >       FORTRAN D
       >        PVM (works with F77 to provide a parallel env.)

       >Does anyone know where we can get information on the
       >above programming environments or any others that may
       >be appropriate?

       Fortran90 is an ANSI and an ISO standard.  The usual reference
       is Fortran 90 Handbook, published by McGraw Hill.  Several vendors
       provide Fortran 90 translators and/or compilers.


HPF
---

         High Performance Fortran (HPF) is a language for programming
       massively parallel architectures. It lets the user insert directives
       for code and data distribution among the processors in the (Fortran
       90) code.

       Electronic copies of HPF draft specification are available
       by anonymous FTP from the following sources:

       Machine name            File name
       -----------------       -----------------------------------
       titan.cs.rice.edu       public/HPFF/draft/hpf-v10-final.tar
       titan.cs.rice.edu       public/HPFF/draft/hpf-v10-final.tar.Z
       titan.cs.rice.edu       public/HPFF/draft/hpf-v10-final.ps
       titan.cs.rice.edu       public/HPFF/draft/hpf-v10-final.ps.Z
       think.com               public/HPFF/hpf-v10-final.ps.Z
       ftp.gmd.de              hpf-europe/hpf-v10-final.ps.Z
       theory.tc.cornell.edu   pub/hpf-v10-final.ps.Z
       minerva.npac.syr.edu    public/hpf-v10-final.tar.Z

       Fortran D is a precursor to HPF; as a commercial product it
       has been superceded by HPF, but several academic projects
       still exist that target Fortran D.

       PVM is a message passing library and run-time environment;
       as such, it exists at a lower level than the previous items.
       One might imagine an HPF processor that produced FORTRAN77
       with calls to PVM.
       There is a newsgroup on PVM.  It is available through netlib,
       and possibly from Oak Ridge as well.

          Hope this
          helps.
          --
          Larry Meadows           The Portland Group
          lfm@pgroup.com


       ----------------------------------------
       From: gale@hpc.pko.dec.com (Israel Gale)
       ----------------------------------------

       Keith,

       Here is a suggestion for your "Parallel Fortran dialects"
       question (Q30) (2.1.5) on your (very useful) Fortran FAQ.

       Larry Meadows' information on HPF is largely correct (except
       for his saying "massively" parallel -- massively parallel is
       the one major parallel architecture for which HPF is not yet
       available), but I thought I'd contribute a few words about
       compiler availability:

       High Performance Fortran (HPF) is an extended version of
       Fortran 90 for parallel programming.  It lets the user insert
       directives into Fortran 90 code which specify the distribution
       of data across processors.

       Currently, most HPF products are not true compilers, but
       source-to-source translators.  Source-to-source translators
       are pre-processors that translate HPF code so that it can be
       compiled by a compiler without native HPF capability.
       They typically output FORTRAN77 source code, with calls to
       a message-passing library such as PVM or MPI.

       Compilers, on the other hand, produce object modules containing
       calls to either a standard message-passing library like PVM or MPI
       (as in the PREPARE compiler currently under development in Europe),
       or to a customized message-passing environment (as in Digital's
       HPF compiler).

       As of May, 1995, the following vendors offered HPF products:

       Compilers                         Source-to-Source Translators
       --------------------------------  -----------------------------
       *Digital
                                         Applied Parallel Research
                                         Hitachi
                                         Intel
                                         Kuck and Associates
                                         Meiko
                                         Motorola
                                         NA Software
       NEC
                                         Pacific Sierra Research
       *PGI
       SofTech

       The first versions of HPF offered a partial implementation known
       as "Subset HPF".  Beginning in 1995, a small number of vendors
       began offering implementations of the full HPF specification.
       Currently, only the vendors marked with an asterisk (*) offer
       full HPF support; all the others support Subset HPF.

       The runtime performance of HPF codes varies widely from vendor
       to vendor.  The best-performing HPF products achieve performance
       comparable to hand-optimized PVM code.


   __________________________________________________________________________
                                       


2.2) Other tools (pretty printers, lints, etc.)



2.2.1) I have heard of fortran "lints" what are they, and where can
       I get one?

       A small "table of contents":

          o  What are Fortran "lints"?
          o  A partial list of "lints"
          o  More info on "lints"
          o  TOOLPACK
          o  NAGWare f77 Tools
          o  NAGWare f90 Tools
          o  lgrind


   What are Fortran "lints"?
   -------------------------
       Fortran compilers are not required (and most do not) to protect
       users from themselves, that is to say:

          call sub(1)
          ...
          subroutine sub(i)
          i=i+10
          return
          end

       Is non-standard complying but the compiler need not tell you
       about it. Arguably worse, the compiler can produce any result
       it deems fit, up to and including the start of world war III
       (assuming the right optional hardware has been installed).

       Fortran lint programs focus on searching out programming errors
       (or likely errors) and alerting the user.

       There are a wide variety of commercial and pd products.



   A partial list of Fortran "lints"
   ---------------------------------

       FORCHECK
          from Leiden University ND 31 71 276804

          "Announcing: The demo of FORCHECK a Fortran development tool.
          The MS-Windows (or WABI) based demo of FORCHECK, a Fortran
          development tool, is now available at simtel as:

             pub/msdos/fortran/fckdemo1.zip  (SimTel Software Repository)

          (primary site oak.oakland.edu).
          (Note: directory names, such as SimTel, are case sensitive.)

          If you are a Fortran programmer it will be a great asset
          in developing portable and reliable code.

             Leiden University
             email: forchk@Rullf2.LeidenUniv.NL
          " end quote

          Actually contrary to the posters claim, this isn't a demo,
          its a hypertext file.  Useful, helpful, but not a demo in
          the usual sense of the word ;> <khb>

       Forwarn
          from quibus 719 527 1384.

       FTNCHEK from netlib.
          One may receive FTNCHEK by mailing
          to:                     netlib@ornl.gov
          the following message:  send ftnchek from fortran

       Glenbrook House
          1/11 Molesey Road
          Hersham
          Surrey, KT12 4RH
          Tel:    0932 88 80 80
          Fax:    0932 88 80 81
          E-mail: les_hatton@prqa.co.u

       HP
          provides a syntax checking facility with their
          Fortran 77 product.

       IPT FORTRAN lint
          1096 East Meadow Circle,
          Palo Alto, CA 94303,
          415/494-7500.

       QA-FORTRAN
          from PRL Programming Research Ltd


       Sun
          provides a syntax checking facility (triggered by Xlist)
          with their Fortran 77 product (3.0.1 and beyond).

       ..................................................
       .  Other vendors (than HP and Sun) also provide  .
       .   syntax checking facilities too, no doubt.    .
       ..................................................



   More info on "lints"
   --------------------

       -------------------------------------------------
       ~from: Ajay Shah, (213)749-8133, ajayshah@usc.edu
       -------------------------------------------------

       You may want to mention f2c followed by an ANSI C compiler as
       a great free fortran lint.  I could not have survived writing
       fortran if it were not for f2c.  You need to know some C to
       deal with the error messages,  but that's not a bad price to pay.


       ---------------------------------------------
       ~From: atae@spva.ph.ic.ac.uk (Ata Etemadi)...
       ---------------------------------------------

       A very kind soul who wishes to remain anonymous sent
       me the answer below.  ...

       1. There is a prettyprinter (called TIDY) available via
          FTP from the SimTel Software Repository (primary site
          oak.oakland.edu).  It's in the directory SimTel/msdos/fortran
          (Note: the directory name SimTel is case sensitive.)

          Capsule review:
          does an ok job, sometimes has trouble with newer extensions
          (and even some Fortran 77 standard features).  Not too
          bright about making good continuation-line break decisions.
          Free, and available via FTP, so probably the quickest solution.
          Includes source (in Fortran).

       2. Greg Flint (afc@klaatu.cc.purdue.edu) at Purdue distributes
          a program called CLEAN77.  Pretty good (higher quality than
          #1 above), also free, but must be obtained from Purdue (not
          available via FTP, not redistributable).
          Available for assorted systems: PC, UNIX, etc.
          In Fortran, comes with source.

       3. There is an excellent prettyprinter in TOOLPACK - probably
          has more options than any other.  Has trouble with extensions,
          such as long variable names.
          Free, comes in source form, in Fortran.
          TOOLPACK as a whole is pretty huge, and requires some work
          to install, but it might be worth it if you stick to pretty
          much standard Fortran. Distributed commercially for a fee
          by NAG, who may have a new, improved version that is better
          than the free one - I don't really know.
          Available via ftp (see archie for locations)

       4. SPAG, formerly sold by OTG Systems (about $1000 for MS-DOS,
          more for Unix). Its main function is to restructure GOTOs
          into IF-THEN-ELSEs, but it also prettyprints.
          (I think they renamed this within the past year).


             plusFORT  : a suite of tools for FORTRAN programmers
                       : comprising SPAG, GXCHK, QMERGE, CMAKE and others.
             Platforms : MS-DOS, Windows, Unix (various), VMS, NT
             Pricing   : Commercial - from 700 or $1000 :
                       : Educational 40% discount

             Pretty-printer: Many options. Can insert declarations for
                           : implicitly typed symbols. Dead code & redundant
                           : variable removal. Symbol name-change option.
                           : Can use case to highlight symbol type.
                           : Also many F66F77F90 conversions.
             Restructuring : Re-organises spaghetti code using block IF,
                           : DO WHILE etc.
                           : Moves code-blocks to minimise control jumps.
                           : Can duplicate code where this helps.
                           : Before & after complexity metrics.
             Static Anal.  : Comprehensive global COMMON block & argument
                           : checks. Identifies globally unused, used but
                           : not set & set but not used. System documentation
                           : & call-tree.
                           : Interactive access to static analysis database.
             Dynamic Anal. : Insert probes in source code to detect the use
                           : of unassigned variables, array elements & char
                           : substrings at run-time.
             Coverage Anal.: Inserts probes in source code to identify
                           : execution hot-spots, & untested code.
                           : Accumulates usage over a series of runs.
                           : Annotates source files.
             CMAKE         : A bit like make, but doesn't need a make-file.
                           : Automatically works out INCLUDE file dependencies.
             QMERGE        : Tool for dealing with system-dependent code.

             Polyhedron Software Ltd.
             Linden House
             93 High St.               Tel:        +44(0)1865-300579
             Standlake                 Fax:        +44(0)1865-300232
             WITNEY                    Compuserve: 100013,461
             OX8 7RH                   Internet:   John@polyhdrn.demon.co.uk
             United Kingdom

       5.  FOR-STRUCT, sold by Cobalt Blue.  Also a GOTO restructurer
           that prettyprints.  About $700 for MS-DOS.  Available from
           most of the big PC software dealers (Programmer's Paradise, etc...)

           (They now have a "budget" version that costs about $250 but
           has program-size limitations.)
           http://www.cobalt-blue.com/ sales@cobalt-blue.com
           (also marketing@cobalt-blue.com)

       6.  PRETTY, sold by Quibus Enterprises, Inc.  Restructures GOTOs,
           also indents, relabels, moves Formats, etc. $149 for MS-DOS,
           $500 for Unix workstations.  Call (719) 527-1384 for more info.



   TOOLPACK
   --------

       -------------------------------------------------------------
       ~From: "John D.  McCalpin" <mccalpin@perelandra.cms.udel.edu>
       -------------------------------------------------------------

       Not too many people use it, but you might want to add TOOLPACK
       to the list of FORTRAN "lint" packages.  Here is the blurb that
       I send to people who are interested:

       TOOLPACK is a large set of utilities written in FORTRAN to do
       FORTRAN code analysis and transformation.

       TOOLPACK begins by actually parsing the program with a fully
       FORTRAN- compliant parser and then does all the code transformations
       on the parse and comment trees.

       This means that you cannot confuse TOOLPACK by silly FORTRAN-isms
       that can easily overwhelm more naive utilities (such as ftnchek).
       For example, TOOLPACK correctly handles statements such as:

             D O U B L E  P R E C I S I O N A(100,100)
             doubleprecision fred

             DO I = 1.2
             READ(I,J) = 10.


       The usual interface to TOOLPACK is a set of 'csh' scripts that
       run the various TOOLPACK utilities to do specific tasks.

       The ones you will find most useful are: pol, polx, apt, dapt,
       decs, getlst, and discard.  These are the prettyprinter,
       precision converter, declaration standardizer, and some
       necessary utilities. See below for more details.

       By aware that TOOLPACK is *very* rigorous about the FORTRAN-77
       standard.  You may or may not consider this an advantage.

       The scripts are described by the 'scripts' script, which delivers
       the following:
       -----------------------------------------------------------------
       In the Toolpack script summaries below, the section numbers refer
       to the Unix environment Users' Guide where more detailed information
       can be found.  To obtain on-line information about a script's usage,
       type its name without any arguments.


       FORTRAN Analysis Facilities

          getlst   Produce a listing showing statement and token numbers.
                   Report lexical scanning warnings and errors. (3.1.1)

          syn     Report errors and warnings detected by lexical scanning,
                  parsing, and examining a set of symbol attributes. (3.1.2)

          sem     Report errors and warnings detected by lexical scanning,
                  parsing, and examining an extended set of symbol attributes.
                  (3.1.3)

          pfort   Report errors and warnings detected by lexical scanning,
                  parsing, examining an extended set of symbol attributes,
                  checking for unsafe references, and checking conformance
                  to a portable subset of FORTRAN. (3.1.4)

          statdoc In a user-supplied report template, place information
                  derived from static analysis to assist in documenting
                  the program.  Examples of information the user may
                  request are COMMON block usage, symbol attributes,
                  and a graph of subprogram calls. (3.1.5)

          inst    Instrument a FORTRAN program so that the instrumented
                  program, when executed, produces information about
                  program execution. (3.2.1)

          rundoc  Execute a program instrumented by inst and, in a
                  user-supplied report template, place information
                  derived from dynamic analysis to assist in documenting
                  the program.  For example, the user may determine the
                  frequency of execution of program segments. (3.2.2)


       FORTRAN Transformation Facilities

          pol     Format a FORTRAN program under control of user-supplied
                  options in a Polish option file. (4.1.1)

          polx    Construct a Polish option file via a menu-driven editor.
                  (4.1.2)

          decs    Rebuild the declarative part of a FORTRAN program. (4.2.1)

          apt     Transform a single-precision version of a FORTRAN program
                  to double precision or vice versa.  (4.3.1)

          dapt    Convert precision and rebuild the declarations, combining
                  the functions of apt and decs. (4.3.2)

          cname   Change the names in a FORTRAN program that satisfy
                  conditions derived from information in either the lexical
                  token stream or the symbol table or both. (4.4.1)

          lname   Transform a FORTRAN program containing long names to a
                  program with standard names. (4.4.2)

          stf     Rebuild the flow of control in a FORTRAN program to
                  standardized form. (4.5.1)

          ucs     Transform nests of DO loops matching certain paradigms
                  so that the transformed code executes more efficiently
                  on vector machines. (4.6.1)


       Miscellaneous Facilities

          fdiff   Compare two FORTRAN programs at the lexical token
                  level. (5.1.1)

          dac     Compare two data files, neglecting certain formatting
                  differences and numerical differences smaller than a
                  given tolerance. (5.1.2)

          vcon    Create, edit, and retrieve versions of a file contained
                  in a version file. (5.2.1)

          discard Remove unneeded files created by the above scripts. (5.3.1)

          scripts Print this summary of the scripts.  (5.4.1)

       ---------

       TOOLPACK can be obtained by anonymous ftp from:

          host:       perelandra.cms.udel.edu
          directory:  pub/Lang/Toolpack/

       The UNIX version is in the file:  toolpack.tar.Z

       Serious hackers will want the versions in the Distrib directory.

       The package is known to compile on Silicon Graphics and Sun
       machines, though the Makefile is reasonably braindamaged.

       You will need about 16 MB for the stripped executables on an
       SGI machine.  Figure on double that for compiling the package.....

          Have fun!
          --
          John D. McCalpin
          mccalpin@perelandra.cms.udel.edu
          Assistant Professor
          mccalpin@brahms.udel.edu
          College of Marine Studies, U. Del.
          John.McCalpin@mvs.udel.edu


   NAGWare f77 Tools
   -----------------

       The NAGWare f77 Tools are a development of Toolpack/1 that raises
       it from a public domain distribution service to a fully supported
       NAG product.

       Large parts of the software have been completely rewritten and
       considerable new functionality added, although all the old
       functionality of the analysis and transformational tools is
       still there.

       First released in 1991, the current version,
       Release 2 contains:

          nag_apt     - Arithmetic precision transformation.
          nag_chname  - Token based name changer.
          nag_decs    - Declaration standardiser (can generify intrinsics).
          nag_fcalls  - Call tree generator.
          nag_fxref   - Variable cross-referencer.
          nag_libdoc  - Interface lister.
          nag_lvi     - Local variable initialiser.
          nag_metrics - Software metrics.
          nag_pfort   - Portability verifier.
          nag_polish  - Pretty printer.
          nag_polopt  - Polish option file editor.
          nag_struct  - Restructurer.
          nag_profile - Profiler and report generator.

       The tools are available for most Unix and VMS.

       These are just some of the many improvements and enhancements that
       we have made:

          1. The US Military standard extensions (DO WHILE, ENDDO,
             IMPLICIT NONE, INCLUDE etc.) have been added to the
             familiar Toolpack/1 language definition, but analyser
             tools still report all extensions to the ANSI standard.

          2. The tools have been substantially rewritten to increase
             the execution speed.  Notably the lexer and parser have
             been 100% rewritten to operate faster and give very much
             better error messages and error recovery.

          3. The user interfaces for the tools are integrated well with
             the target operating systems. Access is via Unix scripts
             (or VMS command language) that carry out complete tasks.

             e.g. To invoke the Portability Verifier for a mixture of
             Fortran and Attribute files, with lower case character
             warnings suppressed:

                Unix

                   nag_pfort -nolcwarn a*.f b*.atr

                VAX/VMS

                   nag_pfort/nolcwarn a*.for,b*.atr

             The script calls the semantic analyser for the Fortran
             files and passes the Attribute files straight to the
             Portability Verifier.

             Or, to call the Precision Transform and Declaration
             Standardise in one step:

                Unix

                   nag_apt -decs file.f

                VAX/VMS

                   nag_apt/decs file.for

          4. User oriented documentation is based around the scripts.
             A relatively slim volume provides all the necessary
             information to run the tools.  A step by step introduction
             to each of the tools is provided, with small examples.

          5. The portability verifier has switches that allow groups
             of less serious messages to be suppressed. For example,
             all warnings about use of non standard characters in strings
             can be switched off.

          6. The portability verifier can dump its internal tables to a
             "library file" that can be loaded in a subsequent pfort run.
             This can be used to provide a definition of argument passage
             in a subroutine library to check a program that calls the
             subroutine library. Library files are more compact and more
             efficient than attribute files for this purpose.

          7. Include files are dealt with sensibly by default, the lexer
             knows about the MIL-STD INCLUDE statement and merges include
             files. The polisher, by default, un-includes the included text.
             Nag_decs, again by default, does not declare variables declared
             in include files.

          8. Tools are distributed in executable form only. The installation
             task is therefore minimal.

       We are developing a new option to the Portability Verifier to aid
       in porting to Fortran 90 by allowing Mil. Std. extensions, names
       up to 31 characters, etc, without the usual errors/warnings.


   NAGWare f90 Tools
   -----------------

       These tools make use of the front-end of the NAGWare f90 compiler.
       Currently, only a small suite of tools is offered, but development
       is on-going. Fixed format input is acceptable, but all output is
       free format. Release 2.1 contents are:

          - Pretty printer (polish)
          - Declaration standardiser
          - Precision standardiser (Standardises precision of
            REAL and COMPLEX)
          - Name changer
          - Call Graph Generator
          - Dependency Analyser (Generates Makefile dependencies)
          - Interface Block Builder
          - Use Statement Annotator (Adds an ONLY list to
            USE statements listing imports)

       Also a module builder and polish options editor are provided.

       Release 2.1 has a full Graphical User Interface as well as a
       command line interface.

       Availability: Most Unix (now).

          Best regards and many thanks, Ian.

          Ian Hounam                            Tel: +44 (0)1865 511245
             Software Engineering Group         Fax: +44 (0)1865 311205
             NAG Ltd.
             Wilkinson House
             Jordan Hill Road
             Oxford OX2 8DR
             UK

          NAG Ltd.                              NAG Inc.
             Wilkinson House
             1400 Opus Place
             Jordan Hill Road
             Suite 200
             Oxford OX2 8DR                     Downers Grove
             UK
             IL 60515-5702

          USA
             Email: infodesk@nag.co.uk          Email:  infodesk@nag.com
             Tel: +44 1865 311744               Tel:    +1 708 971 2337
             Fax: +44 1865 311755               Fax:    +1 708 971 2706

          NAGWare Web page:

             http://www.nag.co.uk/1h/nagware.html


   lgrind
   ------

       Aside from code reformatting, there is the other meaning
       of pretty printing ...

       -------------------------------------------
       ~From: James F Hall <james.f.hall@uwrf.edu>
       -------------------------------------------
       ...

       Second, on Q12 in the faq, about available pretty printers for
       Fortran...  Some time ago, I found a pretty printer called "lgrind",
       which converted a Fortran program into LaTeX/TeX.  This text could
       be included in a larger LaTeX/TeX file, or processed immediately.
       I chose not to use this because I found it was not the best use
       of my quota, but others may find it useful.

       Lgrind may be found using an archie search: archie lgrind ;;;;


   __________________________________________________________________________
                                       


2.2.2) Are there pretty printers for FORTRAN? Flowchart generators?

       Yes.

   One such is SPAG: Authors are:

          Polyhedron Software Ltd.
             Linden House
             93 High St.
             Standlake
             WITNEY
             OX8 7RH
             United Kingdom

             Tel:         +44(0)1865-300579
             Fax:         +44(0)1865-300232
             Compuserve:  100013,461
             Internet:    John@polyhdrn.demon.co.uk

       it's part of their plusFORT product. See above.


   Another is Fortran development Tools from Quibus 714 527 1384


   Also FOR_STRUCT from cobalt-blue:

          Cobalt Blue, Inc.,
          555 Sun Valley Drive,
          Suite K-4,
          Roswell, GA 30076

          Tel:     (770) 518-1116,
          Fax:     (770) 640-1182
          E-Mail:  sales@cobalt-blue.com

       These more than pretty print, they optionally restructure your
       code (duplicating code as needed to tidy up strange GOTO lists,
       turning them into IF-THEN chains, and etc.).


   some more:

       ---------------------------------------
       ~From: dappel@grafted.UUCP (Dave Appel)
        uucp: ..!uunet!grafted.UUCP!dappel
       ---------------------------------------

       wg@cbnewsm.att.com (Bill Gieske) writes:
       > I have tons of old FORTRAN
       > code, most of it in upper case, the majority of it not indented.
       > Is there a code beautifier, either PD or $$ that I can run the
       > code through to improve the readability, hence the main-tainability?
       > Reply to me direct.  I will summarize if appropriate.
       > Bill Gieske AT&T Bell Laboratories wg%alux2@att.research.com

       Call "The Connection at 800-336-1166"  and ask for their
       software catalog.

       In their catalog that I have, Sprint 1992, there is an ad on
       page 39 from AutoCASE Technology.
       They have a product called "AutoFLOW-FORTRAN" that lists for $1,995.
       It claims to automatically document your existing source code.
       AutoCASE's number is 408-446-2273.

       On page 93 is an ad from POWERLINE Software Inc.  Their number
       is 800-257-5773, 206-623-9204.  They offer a product called
       SOURCE PRINT+, which they call a code management tool with
       "multi-style formatting with structured code blocking."

       They have a Fortran/Basic version for $169, and a Delux
       Multi-language version for $249.  This program is for
       DOS (MS-DOS presumably) Windows, and OS/2.

          Hope this helps.  Dave Appel


   Hindsight/Fortran Summary:

       Features include the ability to draw an interactive structure
       chart and display coverage, software complexity and performance
       information on the structure chart. There are also code tracing
       features, for instance 3 logic diagrams are produced.
       Common blocks can be traced through the structure charts,
       including specific variables within common blocks.
       Hindsight is excellent for documentation, code inspection,
       and bringing new software engineers up to speed on new code.

       For more information or a free demo copy, contact:

          Rich Fienberg,  National Account Manager
          Advanced Software Automation, Inc.
          3130A Coronado Dr
          Santa Clara, 95054

          Phone: 408 492-1668
          Fax: 408 492-1669
          Free Seminars Fridays 2-4pm
          Email:  rich@hindsight.com

       Alternative contact (if Dan cannot be reached:

          support@hindsight.com


Other tools:

   Refine/FORTRAN  ("re-engineering tool")

       Reasoning Systems Inc
       415 494 6201
       http://www.reasoning.com

       * The Refine Language Tool[tm] Refine/Fortran[tm].

       Customers use Refine/Fortran to analyze their large FORTRAN
       applications and then to better understand these applications.
       They gain enlightenment about their own software by printing
       reports and diagrams.

       They also apply various workbench features to online versions
       of these reports to find out more about their applications,
       including information as to how the pieces _really_ fit
       together per the semantics of FORTRAN.

       There are reports about coding standards violations, variables,
       variable access, subprograms and call graphs, and data flow
       via COMMON and EXTERNAL blocks.  Coming soon: control flow graphs.

       * Software Refinery[tm].

       Refine/Fortran is unique in the marketplace; it's the only
       extensible FORTRAN application analysis tool.
       A customer uses Software Refinery, a product we also sell,
       to add custom analyses or reports or online displays to
       Refine/Fortran.


   fxref:

       pub/fortran/fxref.tar.Z from biome.bio.ns.ca.
       create cross reference of a FORTRAN program.


   CLEAN77:

       CLEAN77 available from Purdue University.
       Mail Greg Flint (afc.klaatu.cc.purdue.edu) for more info.


   TIDY:

       There is a program called TIDY that is available via
       anonymous FTP from simtel20:

       host:       oak.oakland.edu
       directory:  pub/msdos/fortran/
       file:       tidy621.zip


   Cadre:

       ************************************************************************
       Cadre Teamwork

          222 Richmond
          Street
          Providence, RI 02903
          Phone (401) 351-5950   Fax (401)
          351-7380

       Cadre Technologies Inc.  Cadre Teamwork is a large suite
       of integrated CASE tools that run on Unix and VAX platforms.

       Their core products are structured analysis (with real-time extensions)
       and design, information modeling, and an integrated data dictionary.

       More recently, they have added many extensions, including
       a C development environment, C and Fortran reverse engineering
       (build a structure chart from source code), testing tools,
       and others.


   FORTRAN Partner:

       -----------------------------------------------
       ~From: lionel@quark.enet.dec.com (Steve Lionel)
       -----------------------------------------------

       ~Newsgroups: comp.lang.fortran
       ~Subject: Re: Code formatter for FORTRAN
       ~Date: 15 Jun 1994 15:02:38 GMT
       Organization: Digital Equipment Corporation, Nashua NH
       ~Reply-To: lionel@quark.enet.dec.com (Steve Lionel)


       In article <2tn1bf$aod@rcsuna.gmr.com>,
       jgatowsk@rinhp750.gmr.com (Jan Gatowski EN/16) writes:

       |> Does anyone know if there exists a (commercial or freeware)
       |> FORTRAN code indenter/formatter? A friend is faced with
       |> revamping a largely unreadable old code and could use any
       |> available tools to render it more legible.

       While I was at UK DECUS I attended a talk which described a product
       called The FORTRAN Partner which has as its capabilities (according
       to the documemtation I have):

          Screening:       automatically checking whole FORTRAN programs
                           for classes of error not detected by compiler

          Troubleshooting: analysing programmes interactively to expose
                           problems or inconsistencies


          Porting:         moving code to different FORTRAN environments


          Standardising:   converting code to a consistent style and
                           creating a framework for documentation

          Optimising:      optimising code for speed of execution


       The product is available on the following platforms:


          Alliant FX80
          Avalon Vaccelerator AP/30
          Digital VAX (OpenVMS)
          Digital Alpha AXP (OpenVMS)
          HP Risc Processors under Unix
          IBM PC and compatible systems with minimum 80386
             processor and Maths Coprocessor
          IBM Risc System 6000 under AIX
          Parsys Supernode under Idris
          Silicon Graphics MIPS processors under IRIS
          Sun SPARC and compatible under Solaris and SunOS

       The vendor is:

          Software Validation Limited
          PO Box 270
          Swindon SN4 0TQ
          England
          Tel:  +44 (0) 793 740002
          Fax:  +44 (0) 793 740974

       A single workstation/PC price is given as 945 Pounds.
       I don't know what a US price would be.

       One of the claims which impressed me was the ability to understand
       many different syntax variants and convert them to a more standard
       form.  The formatting rules are customizable.  (The optimizations
       consist of inline expansion and loop unrolling.)

       I have not actually tried this product (I just got a demo disc today)
       and this should in no way be considered an endorsement of the
       product by either myself or Digital Equipment Corporation.
       However, it looks like it would be worth considering for
       some applications.
       --

          Steve Lionel                      Mail: lionel@quark.enet.dec.com
          SDT Languages Group               WWW:  http://www.digital.com/info/s
lionel.html
          Digital Equipment Corporation
          110 Spit Brook Road, ZKO2-3/N30
          Nashua, NH 03062-2698
          "Free advice is worth every cent"


   __________________________________________________________________________
                                       


2.2.3) Is there a WEB for Fortran (and what is web anyway)?

       ------------------------------------------------
       ~From: ecmtwhk@ccu1.aukuni.ac.nz (Thomas Koenig)
       ------------------------------------------------

       FWEB is available via anonymous ftp; use archie(above)
       to determine current location(s).


   As for the more general question, what is WEB ....

       WEB is a  "literate" programming system created by Knuth
       (he of reference book fame, and TeX fame, and etc.).

       It permits the programmer to write code and documentation together.
       WEB takes the "high level code and documentation" and creates real
       publishable documentation (using TeX or LaTeX) and compilable code.
       WEB versions for many languages are available.

       Some features of FWEB are:


          1) FWEB is a pretty printer.  Code is pretty printed by
             sending the FWEB file through "fweave" and "TeX".
             fweave inserts TeX control characters around the code for
             pretty printing.  Fweave also collects a cross-referenced
             index of *all* identifiers and prints them at the end of
             the code listing.

          2) FWEB has built in macro preprocessing, which *does*
             understand FORTRAN syntax and code layout rules.
             A line extending beyond column 72 will be broken into
             proper continuation lines.

          3) FWEB is multilingual: it understands C,C++,f77,f90,
             and RatFor.


   __________________________________________________________________________
                                       


2.2.4) Fortran text editors?

       [...]  More generally, Unipress emacs has a Fortran mode.
       There are XEDIT, BRIEF, TPU and EDT clones available on many
       common platforms these days.


       -----------------------------------------------
       ~From: ig25@rz.uni-karlsruhe.de (Thomas Koenig)
       bitnet:  ig25@dkauni2.bitnet
       -----------------------------------------------

       If you use EMACS, you can use M-x fortran-mode.  An extended
       version, which includes the fortran-auto-fill-mode minor mode,
       is available via anonymous ftp from:

          host:       hallc1.cebaf.gov [129.57.32.62]
          directory:  /emacs

       More generally, Unipress emacs has a Fortran mode.
       There are XEDIT, BRIEF, TPU and EDT clones available on many
       common platforms these days.


       ---------------------------------------------
       ~From: B.R.Eggen@Sussex.ac.uk (Bernd R Eggen)
       ---------------------------------------------

       Torbjorn Einarsson has made available Fortran 90 modes for Emacs
       19.x (and xemacs). They are available e.g. from the Mailbase list
       for Fortran 90, comp-fortran-90 from 12/Jan/1995 onwards. I would
       like to express my gratitude to Torbjorn Einarsson for making this
       valuable tool publicly accessible.

       Files can be retrieved either via anonymous
       ftp to:

          host:       mailbase.ac.uk,
          directory:  /pub/lists/comp-fortran-90/files/

       by Gopher and WWW (World Wide Web), URL (Universal Resource
       Locator):

          gopher://nisp.ncl.ac.uk/11/lists-a-e/comp-fortran-90/files

       or by sending an e-mail to:

          mailbase@mailbase.ac.uk,

       containing the command:

          send <listname> <filename>

       (e.g. send comp-fortran-90 f90.el).


       ---------------------------------------------------
       ~From:  John E. Davis   http://space.mit.edu/~davis
       ---------------------------------------------------

       In addition, JED has a Fortran mode that is very much like the
       emacs Fortran mode.  JED also has a very nice EDT emulation and
       runs on MSDOS, Unix, VMS, as well as DEC Alpha systems.

       JED is no longer available from amy.tch.harvard.edu.  It is now
       available in the USA from:

          ftp://space.mit.edu/pub/davis

       and in Europe from:

          ftp://ftp.uni-stuttgart.de:/pub/unix/misc/slang
          ftp://ftp.prz.tu-berlin.de/pub/unix/editors/

       The latest version is 0.97-14.  A .gif image of JED is also
       available from http://space.mit.edu/~davis/images/jed1.gif.

       Despite the fact that the version number is below 1.0, the editor
       is VERY stable--- the version is below 1.0 because I feel that the
       documentation is not quite up to 1.0 levels.

       Here is a partial list of features:

          o  runs under Unix, VMS, and IBMPC (all versions)
             X Window version also available

          o  emacs*, wordstar*, EDT* emulation C, Fortran*, tex*,
             text editing modes

          o  C-like extension language called S-Lang.

          o  user configurable (bind keys, write functions, etc....)

          o  region highlighting (even on character based terminals!)

          o  Syntax highlighting in Beta test (even on character based
             terminals)

          o  8 bit clean, edit binary files too.

          o  rectangular (box) cut/paste

          o  backup and autosave files

          o  full undo

          o  regular expressions

          o  GNU Emacs compatable

          o  info reader* calendar* mail*, elm like rmail*
             (rmail new in 0.95 version) dired directory editor*

          o  automatic horizontal pan/scroll (configurable)

          o  parenthesis matching/blinking

          o  filename, buffername, function name completion

          o  Menu driven for novice users*

          o  incremental search/replace*

          o  sorting

          o  no hardcoded buffer/line limits

          o  multiple windows and buffers

          o  keyboard macros with macro query feature.

          o  buffer mode lines are configurable, e.g., display time,
             line number, etc...

          o  ispell* shell commands and ``interactive'' shell*

       * Note:  these functions are written in the extension language.

          John E. Davis  internet:  davis@amy.tch.harvard.edu
                         bitnet:    davis@ohstpy


   __________________________________________________________________________
                                       


2.2.5) How can I convert an existing FORTRAN 77 program to the free
       form source of Fortran 90?

       Source code conversion program from ftp
       ---------------------------------------

       Many people who start to code in Fortran 90 prefer to do so using
       the new, less restictive, source form. However, a problem arises
       when wanting to modify old FORTRAN 77 code while sticking to the
       new style. To help in this situation, a source code conversion
       program has been written (and well tested) and made availble by
       anonymous ftp.

       Apart from the conversion, the program can:

          o  ensure that blanks are used correctly in the code as they
             are significant with the new source form;

          o  indent DO-loops and IF-blocks;

          o  replace CONTINUE by END DO, where appropriate;

          o  add subprogram names to END statements;

          o  change non-standard length specification syntax,
             like INTEGER*2, to the Fortran 90 equivalent,
             in all contexts (type statements, FUNCTION statements,
             and IMPLICIT statements);

          o  produce an interface block automatically from the
             source code of a procedure - useful to the library
             developer when wishing to use this important new
             facility with an existing library.

       The source code can be obtained by anonymous
       ftp to:

          jkr.cc.rl.ac.uk (130.246.8.23)

       When prompted for a userid, reply with:  anonymous
       and give your name as password.
       The directory is /pub/MandR and the file name is convert.f90.

          Mike Metcalf  (metcalf@cernvm.cern.ch)


   __________________________________________________________________________
                                       


2.2.6) What is preprocessing, how can it help? How can it hurt?

       Preprocessing often refers to usage of a Macro-prepressor
       upon ones source code prior to compilation.

       How can this help?

          It can make it easier to move code between machines.

       How can this hurt?

          It can cause difficulties in compilation of the processed code;
          most (if not all) macro-preprocessors know nothing about Fortran
          syntax and code layout rules.  So, a common problem is that after
          preprocessing some text may be lost past "sacred" column 72.
          Those working with compilers that optionally compile *past* line
          72 should probably employ that option when using a preprocessor.

       Common prepressors are: cpp, m4, and ratfor. Many sites have their
       own custom prepressors. Basic functions are:

          1) definition of a symbol
          2) conditional code selection based on a symbol
          3) substition of a symbol by its definition

       Traditional BSD Unix f77 processors treat a file named foo.F
       (as opposed to foo.f) as one that should be run through cpp
       prior to compilation "automatically".




2.3) Fortran Packages and libraries




2.3.1) Where can I get "foo" (some random package), older posts
       to comp.lang.fortran etc

       ----------------------------------------------------------
       ~From: mroussel@alchemy.chem.utoronto.ca (Marc R. Roussel)
       ----------------------------------------------------------

       Use archie.  archie is an online database of what is available
       and where on the "net". Archie can be used either via telnet
       or by mail. For information about archie send mail to:

          archie@archie.rutgers.edu     subject:  help

       And you will get back copious directions on how to use archie.
       If you prefer interactive experimentation, telnet to:

          archie.rutgers.edu

       and log in as archie.  No password will be required.
       The first thing you will be shown is a list of other archie servers.
       If one of these servers is geographically much closer to you than
       Rutgers, NJ, please disconnect (by typing 'quit') and use that one.
       To save you this step, here is a  list of archie sites:

          archie.rutgers.edu   128.6.18.15     (Rutgers University)
          archie.unl.edu       129.93.1.14     (University of Nebraska
                                                            in Lincoln)
          archie.sura.net      128.167.254.179 (SURAnet archie server)
          archie.ans.net       147.225.1.2     (ANS archie server)
          archie.au            139.130.4.6     (Australian server)
          archie.funet.fi      128.214.6.100   (European server in Finland)
          archie.doc.ic.ac.uk  146.169.11.3    (UK/England server)
          archie.cs.huji.ac.il 132.65.6.15     (Israel server)
          archie.wide.ad.jp    133.4.3.6       (Japanese server)

       I believe that all of these servers run the mail server as well
       as the telnet and archie server software.  (The archie server
       is a third way to use archie.  It's probably the best way,
       but it requires that you install software.)

       Once you logged into an archie server, you will want to make
       sure that all the information you will retrieve will be mailed
       to you. Type:

          set mailto userid@machine.foo.edu

       where, of course, you will substitute your own email address
       for the made-up one shown above.  You are now ready to search
       the database. If at any time you want to know what options are
       available to you, type help.  To search for a program or file,
       type:

          prog foo

       where foo is the name of the program or file required.
       Once your search is done, type 'mail' to have the output sent
       to you. (The output will almost always be several pages long.)
       Then type 'quit' to exit.



       comp.lang.fortran archives
       --------------------------

       Dejanews archives all Usenet newsgroups, a convenient "entry
       point" for browsing news is:

          http://www.dejanews.com/toplevel.html

       Older news items (more than three months) are kept separatly.


   __________________________________________________________________________
                                       


2.3.2) Where can I find coded BLAS (and what are coded BLAS?)

       The BLAS (basic linear algebra software) comes in several
       flavors:  BLAS-1, -2, and -3.  These can be described as
       scalar, vector and matrix-matrix levels.

       "Coded" BLAS are either hand coded in assembler, or at
       least tweaked for a given machine.

       Some vendors provide these, some are provided on the net
       (see archie) and some are marketed by various commercial
       organizations.

       In addition, it should be noted that BLAS-3 is very amenable
       to parallel processing. Done cleverly, this could be done by
       a network of processors over a net.

       DSS markets just such an implementation. Contact the folks
       below. The following material is their marketing blurb:


          DSSLIB is the fastest BLAS[123], LAPACK, LINPACK, FFTPACK,
          and VFFTPACK available for the entire SPARC hardware and
          software line.

          DSSLIB is based on LAPACK 2.0, but is backward compatible with
          all previous LAPACKs.

          Single-CPU optimization typically yields 2x-4x over Netlib code.
          MP computation yields significantly better than that, reaching
          almost half a gigaflop on a top-of-the-line Sun MP machine and
          exceeding even that on SPARC MP supercomputers.

          Interfaces are shipped with DSSLIB to allow users of IMSL/Math,
          Rogue Wave's math libraries, IDL from Research Systems,
          and others to optimize and parallelize their applications
          without making source code changes.

          The company can be contacted at: Dakota Scientific Software, Inc.
          2241 Cedar Drive Rapid City, SD 57702-3245

             sales@scisoft.com
             +1.800.641.8851  voice
             +1.605.394.8851  voice
             +1.605.348.9623  fax


   __________________________________________________________________________
                                       


2.3.3) Where can I get mathematical software

       There are, of course, many commerical operations which provide
       high quality software. NAG and IMSL to name just two.

       netlib and archie (mentioned above) can be used to good effect
       to find specific freeware (public domain, shareware or mostly
       freely distributable source).

       In addition, NASA's COSMIC distributes some government funded
       software.

       One particular bit of NASA software, MATH77 a large math library
       created by numerical analysts at JPL is available from:

          Language Systems Corp.
          441 Carlisle Dr.
          Herndon, VA 22070
          tel:    (800) 252-6479
          email:  langsys@aol.com


       An excellent place to look for such things is the Web page
       of Tomasz Plewa:

          http://tonic.physics.sunysb.edu/docs/num_meth.html
          http://www.math.psu.edu/dna/num_methods.html
          http://zar.unizar.es/www/num_meth.html
          http://www.labyrinth.net.au/~ctrans/tomasz.html


   __________________________________________________________________________
                                       


2.3.4) What Interval Arithmetic Packages are available?

       --------------------------------------------
       ~From: molagnon@marathon.ifremer.fr
       (Michel Olagnon, Ifremer DITI GO, 98.22.41.4
       --------------------------------------------

       The CADNA package implements stochastic arithmetic (a sort of
       interval arithmetic) in Fortran 90 on the top of any standard
       Fortran 77 program.  That is, if you have a working Fortran 77
       program, you can use CADNA to see what results you get with
       stochastic arithmetic.

       For information on CADNA, or a demo version,
       contact:

          Mr. F. CHAUVET or Mr. BERTHON
          AERO
          3 Avenue de l'Opera
          75001
          PARIS
          tel:  +33 1 44 55 30 80
          fax:  +33 1 40 15 95 54

       For information on stochastic arithmetic (similar to interval
       arithmetic, but the intervals are the most probable error bounds
       instead of the maximum bounds), refer to:

       Vignes, Jean,
       A stochastic arithmetic for reliable scientific
       computation MATCOM 940
       -- Mathematics and Computers in Simulation 35 (1993) 233-261.



       ----------------------------------------------------
       ~From: ig25@fg30.rz.uni-karlsruhe.de (Thomas Koenig)
       ~Reply-To: Thomas.Koenig@ciw.uni-karlsruhe.de
       ----------------------------------------------------

       You might try the XSC series of languages developed at
       the Institute for Applied Mathematics at the University
       of Karlsruhe (look at:

          http://ma20.rz.uni-karlsruhe.de/~ae08/iam/html/xsc-sprachen.html

       if you've got access to Mosaic), or send mail to:

          ae08@rz.uni-karlsruhe.de

       (Rolf Hammer) for more information.

       I'm fairly sure about Pascal, C, and C++; I also believe
       IBM sells a compiler based and their VS series of compilers.


   __________________________________________________________________________
                                       


2.3.5) FLIB Announcement ... Freeware

       Date: Mon, 22 May 1995 19:39:41
       Organization: Kansas State University
       Lines: 93
       Message-ID: <robs.16.0013A98D@ksu.ksu.edu>
       NNTP-Posting-Host: s20.slip.ksu.edu
       Keywords: FORTRAN Freeware
       X-Newsreader: Trumpet for Windows [Version 1.0 Rev A]

       Hello FORTRAN People, This is the first general announcement
       of the FORTRAN Library (FLIB).
       One of the unique aspects of this code repository is that a
       considerable amount of source code is available for non-numeric
       tasks, .e.g.,

           string manipulation,
           time and date functions,
           conversion of numbers to strings (and vice versa),
           etc...

       Many of these tasks are among the most Frequently Asked
       Questions (FAQ) in the FORTRAN usenet group.

       The preferred (by me) method of accessing FLIB is through the
       World Wide Web. The information and code descriptions provided
       via the web will be more up-to-date and comprehensive, and it
       will be easier for you to maintain a stable link to this code
       repository if you access it via the uniform resource locator
       (URL):

          http://www.engg.ksu.edu/~robs/flib/flib.html

       FLIB can also be reached by generic file transfer protocol (ftp).
       If you have trouble accessing FLIB via your web client,
       try using a generic ftp program to access the anonymous
       ftp server at:

          godiva.ne.ksu.edu

       Login as anonymous and enter your email address
       (e.g., robs@ksu.ksu.edu) as the password.
       The flib files are under the directory ~pub/robs/flib.

       The current scope of the code in FLIB is summarized below.
       Please feel free to send me an email message describing your
       opinion/experience with FLIB (remember however that this is
       freeware).

       Rob Stewart  robs@ksu.ksu.edu

       ------------------------------------------------------------
       Scope of Code Repository

       The FLIB routines are currently divided into five areas:

       CharPak

          This package contains approximately 50 routines to
          manipulate character strings (e.g., upper to lowercase,
          removal of specific characters from a string, macro
          substitution). convert numbers  to strings and vice versa,
          align/center text in specific columns,  plus more...


       GeomPak

          For now this package contains less than 10 routines; basic
          routines are provided to scale, rotate, and translate points
          between coordinate systems.  These routines are quite useful
          in a number of computer simulations involving 2 and
          3-dimensional geometries -- including graphics.


       RanPak

          This package contains approximately 30 routines to generate
          random numbers sample from various probability density
          functions (pdf) including a disk, plate, box, sphere, and
          unit direction vectors from arbitrarily oriented cones
          (NOTE: some routines call routines from GeomPak). All of the
          algorithms for random number genration are based on the
          discussion of Lehmer generators (circa 1951) in the article

          Park, S.K. and Miller, K.W.,
          Random number generators: good ones are hard to find.
          Communications of the ACM, 31, No 10 (Oct. 1988).


       TimPak

          A set of routines to access and manipulate the system time
          and date, compute the elapased time between two events,
          etc...  Since most of these routines are system and compiler
          dependent, you will also need to select the appropriate file
          from the Compiler Abstraction Layer (CAL) -- see below.


       Compiler Abstraction Layer (CAL)

          A set of stubs or wrappers for widely used but non-portable
          and non-standard system calls or routines (e.g., system time
          and date).


       Rob Stewart robs@ksu.ksu.edu --or--
       http://www.engg.ksu.edu/~robs/home.html

       Diplomacy: The art of saying "nice doggie" until you can find a rock.



  ;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;



3.1) Fortran and other languages (Essentially C)


3.1.1) "Why do people use FORTRAN?, C is so much better"

       One should avoid such pointless arguments .... if you feel
       this way, don't subscribe to comp.lang.fortran.

       This sort of question always triggers off a protracted
       discussion, the highlights of which are typically:

       a) FORTRAN and C have different semantics. A FORTRAN optimizer
          knows more about aliasing, function interactions, and I/O.
          A C optimizer has to infer or compute such information.
          C bigots typically have neither written such optimizers nor
          worked with folks who do it for a living, and are prone to
          dismiss such arguments as being petty and neolithic.

          FORTRAN programmers are often a bit more in touch with high
          performance computing, and are unwilling to bet that heavily
          on compiler wizardry.

          <enter Peter van der Linden author of "Expert C Programming" >

          In addition, ANSI C section 2.1.2.3 on Program Execution
          makes it clear that associative and commutative regrouping
          of operands is only allowed if it produces the same result
          as it would if the regrouping had not been done.
          Where it makes a difference is on hardware that produces
          an exception on arithmetic overflow, and the regrouping
          either causes or avoids an exception,
          that otherwise would not/would take place.  In ANSI C

             a = a + 32760 + b

          MUST be evaluated as  (a + 32760) + b  NOT as  a +(32760 + b)
          UNLESS the overflow exception will be the same in either case.

          Fortran is somewhat less tightly-buttoned about this, and
          allows the compiler-writer to regroup the expression and
          evaluate it in either order. Thus, in Fortran, whether you
          get an exception or not depends on the compiler, the level
          of optimization, and the hardware.  In ANSI C, it only depends
          on the hardware.

          Of course, compiler options, vendor extensions and the like
          sometimes narrow the difference. Also, some Fortran compilers
          do not take advantage of all of these features of the language,
          thus narrowing the gap in the other direction.

          On any given code, on any given system, all bets are off.

       b) There is a vast body of existing FORTRAN code (much of which
          is publically available and of high quality). Numerical codes
          are particularly difficult to "vet", scientific establishments
          usually do not have large otherwise idle programming staffs, etc.
          so massive recoding into any new language is typically resisted
          quite strongly.

       c) Fortran tends to meet some of the needs of scientists better.
          Most notably, it has built in support for: - variable dimension
          array arguments in subroutines - a compiler-supported infix
          exponentiation operator which is generic with respect to both
          precision and type, *and* which is generally handled very
          efficiently or the commonly occuring special case
          floating-point**small-integer - complex arithmetic -
          generic-precision intrinsic functions

       d) Retraining staff is quite expensive.

       e) It is sometimes argued that: - Jonathan Thornburg <also
          responsible for misc. other fixups>

          Fortran tends to be easier for non-experts to learn than C,
          because its "mental model of the computer" is much simpler.
          For example, in Fortran the programmer can generally avoid
          learning about pointers and memory addresses, while these
          are essential in C.

          More generally, in Fortran the difference between (C notation)
          x, &x, and often even *x is basically hidden, while in C
          it's exposed.  For non-experts this makes Fortran
          a considerably simpler language.

          Because of this relative simplicity, for simple programming
          tasks which fall within its domain, (say writing a simple
          least-squares fitting routine), Fortran generally requires
          much less computer science knowledge of the programmer than
          C does, and is thus much easier to use.


       An interesting (pro-Fortran 90) viewpoint on this subject from
       a practical point of view can be found at:

          http://www.hp.com/wsg/ssa/fortran/f90prent.html

       It's called "Fortran 90 as a language of choice for engineering
       students", and was written by Dr. John K. Prentice from Quetzal
       Computational Associates (Email: john@quetzalcoatl.com).


   __________________________________________________________________________
                                       


3.1.2) Why are there aimless debates?

       There are some persistent individuals who would like computer
       systems to work in a fashion somewhat unlike they do now.
       It seems pointless to debate with them; the debates (in
       various groups) always take the same form and never result
       in meaningful dialog.

       One can usually recognize such by reading a week or so's worth
       of postings. Sometimes you may have to read for a month to
       recognize such. When you do, please try to avoid triggering
       (or responding to) such individuals.

       Many (if not most) newsreaders support a feature entitled
       KILL files.  As you recognize individuals, you may wish to
       put them into your local kill file.
       For example, the style employed by GNUS:

          (gnus-kill "From" "dweeb@place.ISP")
          (gnus-kill "Subject" "test")

       the first kills off all postings from the named individual,
       the second kills off all postings including the beloved
       "test" string. See your local NewsGod for details suitable
       for your local system.


   __________________________________________________________________________
                                       


3.1.3) How do I call f77 from C (and visa versa) This is quite
       platform dependent.

       For Suns see the FORTRAN User's Guide, Chapter 14.

       There is a package available from usenet which attempts
       to make this "quick and easy" for a wide range
       of platforms:

          Host      ftp.germany.eu.net
          Location: /newsarchive/comp.sources.misc/volume20 DIRECTORY
                                   drwxr-xr-x 512 Jul 7 1993 cfortran

          Host      ftp.sunet.se
          Location: /pub/usenet/comp.sources.misc/volume20 DIRECTORY
                                 drwxrwxr-x 512 May 28 1993 cfortran

          Host      ftp.wustl.edu
          Location: /usenet/comp.sources.misc/volume20 DIRECTORY
                           drwxr-xr-x 8192 Oct 30 15:09 cfortran

          Host      halcyon.com
          Location: /dec/.0/usenet/comp.sources.misc/volume20 DIRECTORY
                                     dr-xr-xr-x 512 Jul 8 1993 cfortran

          Host      lth.se
          Location: /pub/netnews/sources.misc/volume20 DIRECTORY
                              drwxr-xr-x 512 Jun 7 1993 cfortran

          Host      math.mps.ohio-state.edu
          Location: /pub/archives/comp.sources.misc/vol20 DIRECTORY
                                 drwxrwxr-x 512 Jun 2 1993 cfortran


       It is on many other sites (around the world) too.
       See archie if you need other pointers.

       For some systems, you have to initialize a runtime system
       explicitly if you call a different language, and stopping
       execution from the other program may not work.


       The most recent version of cfortran.h is available
       via anon. ftp from:

          host:  zebra.desy.de.

;;;;

       ----------------------------------------
       ~From: vankemme@imec.be (Rudi Vankemmel)
       ----------------------------------------

       Yongtao Chen (yongtao@watnow.uwaterloo.ca) wrote:
       : .......
       : * How to call NAG Fortran Library with C (under Unix) ? *

       : We have a NAG Fortran Library on our machine but I do not
       : know how to call them in my C program.  Can anybody give
       : me some advice about how to do this?

       Hello, we have some programs written in C calling the NAG library
       (which is written in Fortran). There are a number of important
       things you must be aware of:

       1) Fortran uses a column wise storage of matrices while C stores
          them row wise. This means that when you want to parse a matrix
          from your C-program to the NAG (-fortran-) routine you must
          transpose the matrix in your program before entering the routine.
          Of course, any output from such a routine must be transposed again.

          If you ommit this step, then probably your program will run
          (because it has data to compute on) but it will generate wrong
          answers.

          B.T.W. if you have the Fortran source code (of any routine)
          then on some platforms you may use compiler directives specifying
          that the Fortran compiler must use row wise storage.
          Some platforms support these directives. However watch out with
          this if you call the same routine from another Fortran
          routine/program.

       2) Your Fortran compiler may add an underscore "_" to the routine
          name in the symbol table e.g. subroutine example(..,..,..)
          becomes example_ in the table.  Hence in the calling
          C-program/routine you must add a trailing underscore !
          Otherwise the loader will complain about an undefined symbol
          "example" while "example_" is loaded.

          However, check your compiler for this. For example the Fortran
          compiler on VAX-VMS systems does NOT add a trailing underscore
          (there watch out with the fact that the VAX-Fortran compiler
          translates everything in uppercase).

       3) Fortran passes its variables by reference. This means that you
          MUST give adresses in your calling C-program (i know, this is
          a stupid remark but it is too often forgotten (my experience ....)).

       4) Watch out especially with float's and double's. Make sure that
          the size of the variable in the calling program is identical to
          the size in the Fortran routine e.g.

             double <----> real*8,
             float  <----> real

          This is extremely important on machines with little endian byte
          ordening.  Parsing a float (C-routine) to a real*8 (Fortran)
          number will not generate SEGV but give wrong results as the data
          is parsed wrongly.


       5) Remember that the array index in Fortran starts at 1 while in C
          this is at index 0; hence a parsed array fortran_array[1:100]
          must be used in the C-routine/program as c_array[0:99].

          Good luck with it !!  Rudi Vankemmel


   another post:


       ---------------------------------------------------
       ~From: beardsl@mepsi.mobil.com (Reginald Beardsley)
       ---------------------------------------------------

       I do a lot of this.  The following is true on the following
       machines.  I cannot say about others.

             Sun 3 & 4 IBM
             RS/6000
             SGI
             DECstation
             Intergraph Clipper (Apogee & Green Hills compilers)
             H-P 7xx

       1) If possible, do not pass strings to FORTRAN from C or vice versa.

       2) Do not mix I/O on the same file descriptors.

       3) Do all your math in FORTRAN, and all the rest in C
          if at all possible.

       4) NEVER ever attempt to write the equivalent of a FORTRAN
          function that returns  a character variable in C.
          Life is too short for the suffering it causes.

       5) If you do ANY I/O in FORTRAN, you MUST use a FORTRAN mainprogram.

       6) FORTRAN always passes pointers. <not necessarily khb>

       7) FORTRAN passes string lengths BY VALUE in the order the
          strings appear in the argument list.  These do NOT appear
          in the FORTRAN argument list, but will appear in the C
          argument list.

       8) You will need to take care of nulls and blanks spaces
          explicitly if you ignor

       9) The Sun FORTRAN compiler used lex and yacc to do the conversion
          of a run time format from a character variable.  If you use
          lex and yacc either rename the variables and functions or
          partially link before you link to the FORTRAN libraries.

       10) FORTRAN symbols have trailing underscores appended.
           Some compilers require a compiler flag to get this.
           Use it! It makes the code more portable.

       11) Don't pass structures.  If you must access a structure element,
           pass a pointer through to a routine which passes back the
           element pointer.

       12) Don't forget that the storage orders for arrays is opposite
           and transposition is expensive.

       I currently have many lines of code with FORTRAN calling C calling
       FORTRAN.  It's not my choice of things to do, but it works well.
       Much better than using the wrong language for the task.  My only
       regret is that I'm forced to pass a lot of strings between the two
       languages.

       Reginald H. Beardsley  beardsl@dal.mobil.com


   followup to first post:


       -------------------------------------------
       ~From: andrew@rentec.com (Andrew Mullhaupt)
       -------------------------------------------

       In article <C9JnIF.Mzp@bernina.ethz.ch>
       brech@vision.ethz.ch (Christian Brechbue

       > It is important that you know what's happening when Fortran
       > and C access array elements.  But I never had to perform
       > any "transposition" step in a program.  You just have to
       > read the definitions the other way.  When the manual says
       > A(j+1,i+1) I understand this means a[i][j] in C, etc.

       This is true enough, but there are times when you don't want
       to modify already existing FORTRAN and C you may have to write
       a transposition wrapper.

       This can be advisable for reasons of clarity (i.e. keeping the
       documentation the code and the math in sync.) and for reasons
       of performance.

       Later,
       Andrew Mullhaupt

;;;;

       Most vendors have surprisingly complete documentation of this sort
       of thing ... if one troubles to look for it. There is, for example,
       an entire chapter in the SunPro Fortran documentation <khb>


   __________________________________________________________________________
                                       


3.1.4) For whatever reasons, I want to translate my Fortran into C.
       What tools are available?

       f90 from NAG, see above

       f2c see above.

       FORTRAN=C=FORTRIX=Rapitech Rapitech (914) 368-3000

       FORTRAN=C=FOR_C=Cobalt Blue  404 518 1116
                                    tel:    (770) 518-1116,
                                    Fax:    (770) 640-1182
                                    E-Mail: sales@cobalt-blue.com

       FORTRAN=C=PROMULA.FORTRAN=Promula (614) 263-5512


   __________________________________________________________________________
                                       


3.1.5) For whatever reasons, I want to translate my existing C code
       into Fortran. What tools are available?

       Regretably none. This is indeed unfortunate, as even a limited
       translator could help with typical C header files.


   __________________________________________________________________________
                                       


3.2) Compiler and system differences



3.2.1) My compiler is mis-behaving; who enforces the standard?

       ANSI and ISO standards do not usually have a particular
       enforcement mechanism. Local bodies sometimes do.

       However, it should be borne in mind that if *your* source code
       is not standard compliant there is *NO* obligation for a FORTRAN
       ('77 and before) compiler to do *ANYTHING* in particular.
       In Fortran (90) the text in "constraints" must be tested and a
       warning produced (compiler option can be used to evade this, of course).

       Some (notably Guy Steele, with respect to another standard)
       have noted that when non-standard complying code is encountered,
       a compiler may do *ANYTHING* including initation of Global Warfare.
       Keep this in mind.

       When you do find a bona fide compiler bug, you are generally
       best served by reporting it to the *vendor*. If you neglect to
       tell the vendor, how can you complain about it not being fixed?

       When reporting a *suspected* bug be sure to be quite specific
       about the computer system, operating system rev level (patches
       applied if known) and *compiler*version* (and patches thereof).
       It is very hard for people to read your mind; but they will try.
       The attempts are often entertaining, sometimes helpful, but
       always an inefficient use of people-time and net-bandwidth.


       Also note that it is generally helpful if you cut down the
       example to the smallest size you can.
       Vendors are developers too; the tendency is invest time/money
       where one can get the biggest bang for the buck.


   __________________________________________________________________________
                                       


3.2.2) My F77 program compiled ok on a <system1>, but gives me heaps
       of syntax errors on a <system2>. What's wrong?

       ------------------------------------------------
       ~from: ecmtwhk@ccu1.aukuni.ac.nz (Thomas Koenig)
       ------------------------------------------------

       Most likely, the program was written with a line length greater
       than 72. If your compiler supports it, turn on the option for
       greater line length (e.g.  -e is not uncommon) ;
       otherwise, split up the lines by hand, or via one of those
       pretty-printers/restructing tools mentioned above.


   __________________________________________________________________________
                                       


3.2.3) My F77 program ran ok on a <system1>, but on a <system2>,
       it just gives me strange results. What's wrong?

       -----------------------------------------------------
       Original:   ecmtwhk@ccu1.aukuni.ac.nz (Thomas Koenig)
       Revised by: klassen@sol.uvic.ca (Melvin Klassen)
       -----------------------------------------------------

       There are different reasons why this could happen.  Possibly, your
       program violates the standard in some way which is not caught by the
       compiler on <system1>, or in some way which the compiler on
       <system1> intentionally allowed, e.g., in FORTRAN 77,
       variable-names were restricted to 6 upper-case characters, while
       many compilers were extended to handle longer, mixed-case names.

       Some programs rely on the retention of values between invocations.
       Use SAVE statements for those variables which you need to keep
       across function calls.

       Some programs rely on variables to be initialized to zero when a
       subroutine or function is first called. Some compilers (VAX/VMS
       for example) exhibit this behaviour.

       Some operating systems (IBM's MVS/ESA and VM/ESA for example)
       have been observed to fill with a "zero" value the first time
       you reference a previously-unused area of virtual storage.

       Compilers on newer architectures often fill variables with
       garbage on each new function call. This is permitted,
       according to the standard.

       The solution is to explicitly initialize all variables.

       Your compiler may have an option to trap uninitialized variables;
       use that to find the trouble spots.  For example, the IBM VS
       compiler will do a static-flow-analysis, and report such errors,
       when you specify the 'OPT(2)' option.  Alternatively, if you are
       desperate, try to compile using a flag which forces static
       allocation of all variables.

       Another problem might be that the accuracy of REAL and DOUBLE
       PRECISION differs between different platforms; that can cause
       roundoff error to wipe out your results or your program to go into
       endless loops.

       Yet another (and much more subtle) problem can occur if a lot of
       formatted I/O is employed. The conversion from internal to external
       representations can introduce very significant errors; much worse on
       some platforms than others (doing correctly rounded base conversion
       is expensive).

       There are, of course, lots of other possibilities, these are just a
       starting point.


   __________________________________________________________________________
                                       


3.2.4) How can I read my VAX binary data somewhere else?

       Some vendors provide bulit in methods (DEC provides this via
       special options on the OPEN statement). Others provide library
       support (on SPARC products, with the SunPro compilers, checkout
       convert_external)

       In addition, Accerl8 provides a commerial tool. Contact:

          Harry Fleury                         Tel: (303)863 8088
          Accelr8 Technology                   Fax: (303)863 1218
          303 E. 17th Ave., Suite 108          Email: harry@accelr8.com
          Denver, Colorado 80203               http://www.accelr8.com


;;;;


   __________________________________________________________________________
                                       


3.3) Language extensions


       The following three Q's and A's based on email from:

          ecmtwhk@ccu1.aukuni.ac.nz (Thomas Koenig)



3.3.1)  How common is DO ... END DO

       It is very common; and of course is part of Fortran 90.
       Compilers claimed to *not* support it
       (much shorter list this way):

          1) Salford ftn77/Primos version

          2) Prime f77 compiler

          3) Microsoft Fortran for CP/M 8080/Z80 machines

          4) Fujitsu VPxxx UXP/M compiler


   __________________________________________________________________________
                                       


3.3.2) What are ENCODE and DECODE statements, and how are they translated
       to standard Fortran? How can I convert numbers to character strings
       (and vice-versa)?

       ENCODE and DECODE are vendor extensions to Fortran (invented in
       the sixties, long before X3.9-1978 added internal I/O to the
       language) which are most often used to convert data between
       numeric and character representations.  They may be viewed as
       formatted writes to (ENCODE) or reads from (DECODE) memory.
       The standard-conforming alternatives are internal write and
       internal read statements respectively.

       For example,

            INTEGER MONTH, DAY, YEAR

            MONTH = 7
            DAY = 4
            YEAR = 93
       C    FORM THE STRING  7/ 4/93 IN VARIABLE "DATE"
            ENCODE (8,10,DATE) MONTH,DAY,YEAR
        10  FORMAT (I2,'/',I2,'/',I2)

       The above can be translated as "write 8 characters, formatted
       according to format 10, storing the results in variable DATE, and
       using the contents of variables MONTH, DAY, and YEAR as the data to
       write."

       A DECODE statement would be used to reverse the process (extract
       the variables MONTH2, DAY2, and YEAR2 from the string DATE).
       Thus:

          INTEGER MONTH2, DAY2, YEAR2
          DECODE (8,20,DATE) MONTH2, DAY2, YEAR2
     20   FORMAT (I2,1X,I2,1X,I2)

       Conversion of ENCODE/DECODE to standard Fortran-77 is not difficult.
       The critical thing to remember is that the variable to be written
       to (ENCODE) or read from (DECODE) must be a CHARACTER variable
       which is long enough to contain the string.
       The first number within the parentheses (in this case 8) is the
       minimum length to use in a type declaration.

       Thus a standard-conforming equivalent of the above
       example is:

           CHARACTER*8 DATE
           INTEGER MONTH, DAY, YEAR

           INTEGER MONTH2, DAY2, YEAR2
           MONTH = 7
           DAY = 4
           YEAR = 93

           WRITE (DATE,10) MONTH, DAY, YEAR
        10 FORMAT (I2,'/',I2,'/',I2)
           READ (DATE,20) MONTH2, DAY2, YEAR2
       20  FORMAT (I2,1X,I2,1X,I2)

       Although the above example used integers, any other data type
       may also be used.

       -----------------------------------------------------
       From: <forags@nature.berkeley.edu (Al Stangenberger)>
       -----------------------------------------------------


   __________________________________________________________________________
                                       


3.4.1) What is involved in parsing Fortran?

       ----------------------------------------
       ~From: clodius@hotspec (William Clodius)
       ----------------------------------------

       > I don't know if the following is any help
       >
       > Dec has published a discussion of some of the problems
       > in parsing Fortran
       > http://www.digital.com/.i/info/hpc/f90/loveman.txt
       >
       > There is a publicly available Fortran90 grammar for a compiler
       > generator at
       >
       > http://www.cs.colorado.edu/~eliuser/fortran_html/Scan.html
       >
       > The "compiler" generator that uses the grammar, ELI,
       > apparently has home pages at
       >
       > http://www.cs.colorado.edu/~eliuser/
       > http://www.uni-paderborn.de/fachbereich/AG/agkastens/index_engl.html
       > http://coral.cs.jcu.edu.au/
       >
       > however the links to Germany and Australia did not work
       > when I tried them out.
       >
       > The Sage++ compiler development system apparently has
       > Fortran 77/M parsers available
       >
       > http://www.extreme.indiana.edu/sage/index.html


       ------------------------------------------------
       ~From: mjohnson@samson.tx.hac.com (Mark Johnson)
       ------------------------------------------------

       > Christian Rutzinger <rutzinger@takefive.co.at> wrote:
       >
       > >I want to write a Recursive Descent Parser for Fortran90. ,,,
       > >
       > >Am I wrong, or is (Standard) Fortran90 really a not
       > >LL(1) language?
       >
       > FORTRAN is definitely not LL(1).  A good example is the difference
       > between the following two statements
       >         DO 10 I=1,10
       > and
       >         DO 10 I=1.10
       > [the real difference is the comma in the first one & the period in
       >  the second example]
       >
       > The first starts a DO loop, using [implicitly integer]
       > I as an index, counting from 1 to 10.
       > [7 tokens - DO, 10, I, =, 1, ",", and 10]
       > The second assigns the value 1.1 to the [implicitly real]
       > variable DO10I. [only 3 tokens - DO10I, =, 1.10]
       >
       > Needless to say, you sometimes have to examine the entire statement
       > before you know what kind it is & generate tokens. One approach to
       > handle this is to do something like...
       >   call read_statement(line)
       >   call statement_type(current_state, new_state, s_type, line)
       >   <computed goto based on s_type, etc.>...
       > where the statement_type procedure uses the "current state" and
       > the input line(s) to determine the statement type "s type" and
       > "new state".  The "current state" and "next state" represent the
       > language rules relating to the order of statements. This solution
       > isn't very efficient, and dumps a lot of functionality into the
       > statement_type procedure. But it is a robust and somewhat easy
       > to describe solution. There are undoubtedly others who could
       > supply more optimal solutions.
       >
       > Good luck on your work.
       >   --Mark
       > --
       > -- Mark Johnson <mjohnson@samson.tx.hac.com>
       > [I put a little Fortran subset parser in the comp.compilers
       > archives several years ago.  It uses a yacc parser and a lot
       > of lexical feedback.  It's not complete, but the structure is
       > adequate to parse all of Fortran. -John]
       >
       > --
       > Send compilers articles to compilers@iecc.com,
       > meta-mail to compilers-request@iecc.com.



  ;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;
                                       


4.1.1) WWW and Fortran

        See http://www.nag.co.uk/nagware/Examples/cgi.f90


       --------------------------------------------------------
       ~From: C.D.H.Williams@exeter.ac.uk (Charles DH Williams)
       --------------------------------------------------------

       > In article <4hmd1k$c0m@cpca3.uea.ac.uk>, "M.W.Gardner ENV PG"
       > <e449> wrote:
       >
       > > Could anyone give me pointers to information concerning
       > > the use of F90 programs as CGI servers.  I wish to write
       > > programs to generate WWW pages interactively. Has anyone
       > > done this ?  If so please contact me.
       > >
       > > I have checked out the FAQ and F90 pages with no success.
       > > I also know that perl is probably a more traditional
       > > language to do this sort of stuff.
       >
       > You may find that John Rowe's "Metaform" system does what you want
       >
       > http://newton.ex.ac.uk/metaform/
       >
       > lets users write and install their own cgi code in whatever
       > language they like without causing security problems et al.
       >
       > I used it to implement a simulation of a temperature control
       > system which takes lots of parameters and draws graphs
       > representing the results. Get to it via the last line in
       > the contents list of
       >
       > http://newton.ex.ac.uk/teaching/CDHW/Feedback/
       >
       > Good luck
       >
       > Charles


       --------------------------------------------------
       ~From: Kavan Ratnatunga
       --------------------------------------------------

       Recently I wrote fairly large cgi-driver in f77 and found that
       it was not very difficult, and for my application since the
       output I was putting on the web was originally created from
       fortran analysis programs, there were some particular advantages
       in the program logic.

       If interested see:

          http://archive.stsci.edu/mds/mds_cgi.f

       Kavan Ratnatunga


   ;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;


