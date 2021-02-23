# OSDtwodotwhoa
# Goals and Summary

This is a refactoring of the Open Source Definition, inspired by work I did some time ago to refactor the Open Knowledge Definition between its version 1 and 2.0, and egged on by real-life discussions at FOSDEM and CopyleftConf in 2020 and on Twitter in 2021.

My primary motivation here is to show what *can* be done to make the OSD more comprehensible and useful. I do not have the time or motivation to shepherd a rewrite through OSI, but since I've done the work I figured I'd share it in hopes it can be useful to someone.

The primary structural changes are two-fold:
* The definition of open source *software* is split from open source *licenses*, resolving a confusion OSI historically inherited from Debian (which as a distributor of software itself, had to answer both questions simultaneously).
* Breaks the definition of an open license into required permissions, forbidden restrictions, and permitted restrictions, each of which are separate concepts but which are intertwingled in the original OSD and DFSG.

## Unavoidable(?) Questions
Refactoring code often exposes questions about the intended behavior of the original code. This refactoring is no different. Two particular questions jump out, but I'm sure others may be lurking:

* **Allowed Restrictions**: The OSD has always explicitly permitted some restrictions, but has remained silent on many others that are present in many licenses. Sections 2.3.1 and 2.3.2 extract OSD's existing language on this topic, while Sections 2.3.3-2.3.6 (and the last clause of 2.3.1) attempt to capture existing permitted restrictions, such as copyleft. This is almost certainly not a comprehensive list, but I've attempted to capture most of the common restrictions. 

* **Explicit Grant of Use**: Licenses must of course allow use, but this is not actually explicit in the current OSD. (It is implied most strongly by OSD #6.) It seemed to me worth saying, so this is now 2.1.1.

## Questions That Are Out Of Scope
This draft does not touch on the extremely important question of how the document should be interpreted. Where should the benefit of the doubt lie? What presumptions should be made about different types of license stewards? How should OSI think about innovation? How should OSI react to groups creating source-available, but likely not OSD-compliant, licensing schemes?

All of these things are out of the scope of this draft refactoring. 

## Stylistic Notes

A few notes on stylistic choices:

* **Examples**: I have chosen to drop most examples. They should move to an FAQ, where they can be updated regularly with examples from license submissions, rather than being static and limited in a document that should be rarely updated. This does *not* imply dislike of any particular examples; in particular, this is not an attempt to sneak in "commercial open" by removing the example of for-profit businesses from OSD #6!
* **Refactor or rewrite?**: When I originally wrote this in 2020, I tried to keep it to a minimalist refactor, making as few changes as possible to the actual text. My increasing frustration with bad drafting in 2021 sparked some more major stylistic changes (though again still with the intent of keeping the substance the same). Most notably, this includes a complete rewrite of Sec. 2.1.3 from an earlier cut/paste pastiche of OSD 1, 3, and 4; and an aggressive simplification of 2.1.2. This may make comparison harder, and invite more conspiracy theorizing about how I'm trying to ruin the OSD somehow.
* **Titles**: I've tried to draft section titles to make them closely parallel the wording of the section. 
* **Parallelism**: I have, wherever possible, tried to create parallelism of language. For example, part of OSD #6 that was "must not restrict" becomes "must allow" in Section 2.1.2. However, more could be done here; for example, I'd love to find a better way to phrase 2.1.4 to make it consistent with the rest of 2.1 (including perhaps accepting that it should be part of Section 1!)
* **Terminology**: I have tried to be consistent in terminology, such as consistent use throughout of "licensed software" rather than "work" or "program".

# Revised OSD
## Summary

*Software is open if anyone is free to access, use, modify, and share it — subject, at most, to measures that preserve provenance and openness.*

The key words “must”, “must not”, “should”, and “may” in this document are to be interpreted as described in [RFC2119](https://tools.ietf.org/html/rfc2119).

## 1. Open Source Software

To be open source, **software** must satisfy the following requirements:

### 1.1 Open License

The complete source code for the **software** *must* be available under an open **license** (as defined in Section 2). Any additional terms accompanying any form of the software (such as terms of use, or patents held by the licensor) *must not* contradict the terms of the license.

### 1.2 Source Available

The source code for the **software** *must* be available to those who receive the software, either distributed with the software or via a well-publicized means for no more than a reasonable reproduction cost.

The source code means the preferred form in which a programmer would modify the software. Deliberately obfuscated source code, or intermediate forms such as preprocessor output, are not allowed.

## 2. Open Licenses

A **license** is open if its terms satisfy the following conditions:

### 2.1 Required Permissions

The **license** *must* grant the following permissions:

#### 2.1.1 Use

The **license** *must* allow use of the licensed software. 

#### 2.1.2 Modification

The **license** *must* allow the modification of the licensed software.

#### 2.1.3 Redistribution

The **license** *must* allow redistribution of the licensed software, whether:
* for a fee or at no cost;
* on its own, or as part of a collection made from software from different sources;
* in source code form or other form; and
* modified or unmodified.

#### 2.1.4 Propagation 

The **license** *must* apply to all to whom the licensed software is redistributed without the need for them to agree to any additional legal terms. 

#### 2.1.5 Separability

The **license** *must* allow any part of the licensed software to be distributed separately from any other part of the licensed software, or from any collection of software with which it was originally distributed.

#### 2.1.6 Subsequent Recipients

The **license** *must* grant all subsequent parties who receive licensed software at least the same rights granted to the original recipients.

### 2.2 Prohibited Restrictions

The **license** *must not* contain any of the following restrictions:

#### 2.2.1 Non-discrimination

The **license** *must not* discriminate against any person or group. 

#### 2.2.2 No Charge

The **license** *must not* condition the permissions in Sec. 2.1 on any fee arrangement, royalty, or other compensation or monetary remuneration.

#### 2.2.3 Application to Any Purpose

The **license** *must not* restrict anyone from using the licensed software in a specific field of endeavor. 

#### 2.2.4 Unrelated Software Distributed Alongside

The **license** *must not* restrict other software that is distributed alongside licensed software.

#### 2.2.5 Technology Neutrality

The **license** *must not* condition the permissions in Sec. 2.1 on a specific technology or style of interface. 

### 2.3 Acceptable Conditions

The **license** *must not* limit the permissions required in Section 2.1, except by the following allowable conditions:

#### 2.3.1 Reputational Integrity

The **license** *may* require that modified software carry a different name or version number from the original software, or otherwise indicate that changes have been made.

*Rationale*: The first part of this section is the third sentence of OSD #4, but an added "or otherwise indicate" clause attempts to capture Apache 2.0 4.b and GPL 2 2.a.

#### 2.3.2 Source Code Integrity
The **license** *may* restrict source code from being distributed in modified form, if the license allows the distribution of "patch files" with the source code for the purpose of modifying the program at build time.

#### 2.3.3 Attribution

The **license** *may* require retention and conveyance of copyright notices and license texts to recipients of the licensed software.

*Rationale*: This is an attempt to capture various notice and attribution requirements.

#### 2.3.4 Share-alike 

The **license** *may* require copies or modifications of the licensed software, including executable forms, to be distributed under the same license as the original licensed software.

The **license** *may* require distribution of the licensed software's source code to recipients of executable forms of the licensed software.

*Rationale:* This is an attempt to capture the core intutions and mechanisms of copyleft.

#### 2.3.5 Technical Restriction Prohibition

The **license** *may* prohibit distribution of the licensed software in a manner where technical measures impose restrictions on the exercise of otherwise allowed rights.

*Rationale*: This is an attempt to capture GPL v3's DRM clauses. However, it is possible that it may be better seen as an instance of "otherwise aggressing" in Sec. 2.3.6, and used as an illustrative example in an FAQ.

#### 2.3.6 Non-aggression 

The **license** *may* condition a licensee's permissions on not litigating or otherwise aggressing against licensors or other licensees, in an attempt to prohibit the exercise of any grant allowed by the license.

*Rationale:* This is an attempt to capture patent defense clauses present in many OSI-approved licenses, dating back to the Netscape Public License.

# Changelog

Unfortunately, I have not found a great way to visually (or otherwise, such as through a git history) show what sections of the former OSD go where in the new draft. This list is provided to allow easy auditing to make sure I didn't miss anything (and indeed, while preparing it, I found two sentences that had been accidentally dropped).

* OSD #1 ("Free Redistribution") 
    * first sentence → 2.1.3
    * second sentence → 2.2.2
* OSD #2 ("Source Code") → 1.2.
    *  This could easily be updated and slimmed down. For example, it is unclear whether there is any such thing as a 'reasonable reproduction cost' in 2021, and I suspect that the definition of source code in this context is now so well-understood that it could be deleted, or moved to an FAQ/annotation. 
    *  I am unclear what it means that "The program must... allow distribution in source code as well as compiled form" (programs don't allow distribution in source code form, rightsholders do?) so that has not been included in this revision.
* OSD #3 ("Derived Works") → 2.1.3
* OSD #4 ("Integrity of the Author's Source Code")
    * first sentence → 2.3.2
    * second sentence → 2.1.3 (modified to make structure parallel to other permissions)
    * third sentence → 2.3.1 (with addition to reflect Apache/GPLv2 requirements)
* OSD #5 ("No Discrimination Against Persons or Groups") → 2.2.1
* OSD #6 ("No Discrimination Against Fields of Endeavor") → 2.2.3
    * In keeping with the drafting note that examples should generally live in an FAQ or annotation, the second sentence has been dropped. This is not intended to endorse discrimination against businesses (or genetic research), but rather to make it easier to update and elaborate on the list of examples.
* OSD #7 ("Distribution of License") → 2.1.4.
    * It's possible that this should either (1) be merged with 2.1.6 or (2) made Sec. 1.3 (i.e., a quality of software rather than of a license)
    * This is a good example of where earlier refactoring would have helped clarify drafting—if this is an attempt to prohibit someone from distributing, say, Netscape Navigator under a clickwrap NDA and calling it open source, then this should be in Sec. 1; if it is an attempt to prohibit clickwrap open source licenses for some other reason, then it should be in Sec. 2.1 but drafted more clearly.
* OSD #8 ("License Must Not Be Specific to a Product") → 2.1.5 and 2.1.6.
    * This entire section could stand to be further edited/rewritten for better parallelism.
    * Like OSD 7/New OSD 2.1.4, the first sentence ("The rights attached to the program...") may be better placed in Sec. 1 instead of Sec. 2.
* OSD #9 ("License Must Not Restrict Other Software") → 2.2.4.
    * Could perhaps be combined with 2.1.3 instead?
    * Again I have removed an example that better belongs (and should be expanded!) in an FAQ or annotation.
* OSD #10 ("License Must Be Technology-Neutral") → 2.2.5.
