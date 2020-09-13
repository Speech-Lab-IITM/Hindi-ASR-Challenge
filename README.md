# Hindi-ASR-Challenge
🎯 Speech Recognition Challenge by Speech Lab - IIT Madras

### Table of Contents
   * [What is this about?](#what-is-this-about)
      * [Guidelines](#guidelines)
      * [Tracks](#tracks)
      * [Important Dates and Timeline](#important-dates-and-timeline)
   * [Get Started](#get-started)
      * [Link to the Data](#link-to-the-data)
      * [Quickstart](#quickstart)
      * [Building Your Own ASR Model](#building-your-own-asr-model)
   * [Get In Touch With Us!](#get-in-touch-with-us)
   * [Citations](#citations)

## What is this about?
This challenge is held to help advance State-of-the-Art performance in Artificial Speech Recognition of Hindi Language
and spread the spirit of research for the same. Conducted by the Speech Processing Lab of IITM under Dr. Umesh S, this challenge
aims at generating transcripts from audio files created by volunteers reading actual news-paper articles. 

This challenge is a part of the [National Language Translation Mission](http://psa.gov.in/pmstiac-missions/natural-language-translation) 
funded by [MeitY](https://meity.gov.in/).

The text data was crawled from newspapers, and then volunteers were asked to read them. It covers genres like politics, 
sports, entertainment, etc. 
The following data sets will be released for this challenge:
- Train Set: 40 hours
- Dev Set: 5 hours
- Test Set - 5 hours 

along with the corresponding transcripts and time-stamps. The challenge is open to all 
irrespective of being individuals, teams or organizations. 

A baseline of GMM-HMM and TDNN models are set up and the pre-trained model weights are available for download (discussed
below). Lexicons, results and recipes to replicate the baseline experiments are also made available.


### Guidelines
- The data can be freely downloaded after registration for the challenge and agreeing to the *License of Fair Use*. The data 
will also be publicly available after the end of the challenge in the good spirit of research, development and 
advancement of the Speech Recognition domain of the Deep Learning community.
- Any additional data can be used for training (public and private) as long as the participant(s) have legal rights over 
it. The Lab and and Institute in no way will be held responsible in any way with respect to copyright claims of the 
participant's data.
- Submissions are to be made [here](https://docs.google.com/forms/d/e/1FAIpQLSe7vUA9hQRCzrnkGYJDKGNULXkdW_ykKlU9Xu4F380sKwrSqw/viewform?fbclid=IwAR3lQ_dS3cBWh6XVYCBCcQml2Yas3ZsH3LNPm1FRqCvH_hELVIvtfdGVBCY). A leaderboard will be maintained regularly and can be checked [here](https://sites.google.com/view/asr-challenge/leaderboard). Submissions 
should include the ASR output produced by the system and a brief description of the system. Participating teams can 
submit a maximum of 10 submissions per team

### Tracks
- **Closed Hindi-ASR Challenge**: Only the training data distributed as part of the challenge can be used to train the 
models (both acoustic and language models)
- **Open Hindi-ASR Challenge**: You can use any external/additional data to train the acoustic and language models.  

Results will be displayed on a leaderboard throughout the period that the submission site is open

### Important Dates and Timeline
- Release of train,dev data: July 6 2020
- Eval data release and opening of submission site: August 21, 2020
- Closing of submission site: August 30, 2020 (midnight anywhere in the world, i.e., 12pm UTC on August 30, 2020)
- Announcement of results: Spetember 4 2020

## Get Started
### Link to the Data
Enroll yourself using the following link: [Register Now!](https://forms.gle/aR7e28YjgB3g5fgW6)

Registering on the above link provides access to the user license and a userud and password to download the training and test data for Hindi challenge.

In case you want to use the terminal for downloading, after getting access to the data, use the command 
```
$ wget --user=<UID> --password=<PWD> -U "" <DOWNLOAD_LINK>
```

### Quickstart
Especially targeted at beginners and participants who would like to get a hand at ASR in practise, a ready to run recipe
notebook on [Binder](https://mybinder.org/) of the pre-trained baseline model is available 
[here](https://mybinder.org/v2/gh/Syzygianinfern0/WAV2TEXT.git/master). The development environment of Kaldi-ASR and all
its required dependencies are already available. Given an audio file, and using the pre-trained weights (already loaded)
, the model would generate the Hindi transcripts.

Please checkout the `quickstart` directory for more information on the model and a downloadable notebook. 

### Building Your Own ASR Model
The code is inherently from [Kaldi-ASR](https://kaldi-asr.org/) and the training scripts can be found under the 
`asr` directory. The pre-trained models from these baseline are also available for download considering if the participants might want to start from a checkpoint.

## Get In Touch With Us!
- If there are any queries or issues, please open a GitHub Issue [here](https://github.com/Speech-Lab-IITM/Hindi-ASR-Challenge/issues/new) so that others with similar queries may also be benefit from the same.
- You can also contact us over mail at speechiitm@ee.iitm.ac.in
 
**Related Links**:

- Challenge Website: https://sites.google.com/view/asr-challenge/home
- Lab Website: https://speechiitm.wixsite.com/sphlab
- Official Site of Dr. Umesh S: http://www.ee.iitm.ac.in/~umeshs/
- Official Institute Link: https://www.iitm.ac.in/

<details> <summary>License and Fair Use</summary> 

### IITM Hindi Speech Corpus: a corpus of native Hindi Speech Corpus Licence Agreement
 
This Agreement is made between Speech lab IITM (Speech-IITM) and the LICENSEE, whereas Speech-IITM , through its 
Research Unit "Speech lab", collected a corpus of speech utterances in various Indian metropolitan cities. This 
agreement refthe IITM Hindi Speech corpus data set, in the following referred to as DATA, which consists of utterances 
and related transcriptions from people aged between 20 and 60. 

The Property Rights of IITM Hindi Speech Corpus DATA are owned by Speech-IITM. The LICENSEE is interested in acquiring 
a license to use IITM Hindi Speech Corpus DATA only for research purposes. It is hereby agreed as follows:

#### 1 - Object
Speech-IITM grants LICENSEE a non exclusive, non transferable, non sublicensable, unlimited, free of cost licence of 
the DATA. LICENSEE will use the DATA for research purposes and agrees that the DATA, in whole or in part, shall not be 
distributed or delivered to any third party.

#### 2 – Property Rights
The licence issued within this Agreement does not confer any title and/or right to LICENSEE on the DATA and, for this 
reason, LICENSEE cannot proceed to any record, assignment and/or concession as sub-license of the named DATA and of the 
relative rights of use. It is expressly understood that the DATA, and the related rights or titles of copyrights able to 
protect completely or partially the DATA, will remain in the whole property of Speech-IITM, and they can be used by 
LICENSEE only for research purposes hereby defined.

#### 3 – Limitation of Warranty and Liability
Speech-IITM makes no representations about the suitability, use, or performance of the DATA for any purpose. The DATA 
are provided “as is,” without express or implied warranties including, but not limited to, any implied warranties of 
merchantability, fitness for a particular purpose, or non-infringement with respect to the DATA. Speech-IITM is not 
obliged to support or issue updates to the DATA. Speech-IITM shall not be liable for any damages, including direct, 
indirect, incidental, special or consequential damages for loss of profits, revenue, data or data use, incurred by 
LICENSEE or any third Party, whether in an action in contract or tort, even if any person has been advised of the 
possibility of such damages.

#### 4 – Duration
The License under this Agreement shall come into force starting from the date hereof. The License will terminate 
immediately, without notice by Speech-IITM, if LICENSEE fails to comply with the terms and conditions of this Agreement. 
Upon termination of this License, LICENSEE shall immediately discontinue all use of DATA provided hereunder, and return 
to Speech-IITM or destroy the original and all copies of all such DATA. All of LICENSEE obligations under this Agreement 
shall survive the termination of the License.

#### 5 - Indemnification
LICENSEE agrees to hold harmless, indemnify, and defend Speech-IITM, its Trustees, officers, employees, and agents from 
and against any loss, damage, liability, claim of loss, lawsuit, cause of action, or other claim asserted against them 
or any of them arising out of, or in any way connected with, LICENSEE performance of any activity hereunder.

#### 6 – Publications Credit
LICENSEE shall acknowledge Speech-IITM with appropriate citations in any publication or any public presentation 
containing results obtained through the use of the DATA as well as to demonstrate the DATA, expressly stating that 
within the Project Speech-IITM has developed and owns the DATA, including a citation to the following publications:

“IITM Hindi Speech Corpus: a corpus of native Hindi Speech Corpus” - Speech signal processing lab, IIT Madras.

#### 7 – Applicable Law
Any controversy or claim of whatsoever nature arising out of or relating in any manner whatsoever to this Agreement or 
any breach of any terms of this Agreement shall be governed by and construed in all respects in accordance with the 
laws of India.

LICENSEE hereby irrevocably acknowledges and agrees that the Court of India shall have India exclusive jurisdiction to 
resolve any controversy or claim of whatsoever nature arising out of, or relating in any manner to this Agreement, any 
terms of this Agreement, or any breach of this Agreement or any such terms.

#### 8 – Privacy regulation

Your personal data shall be processed only for internal usage by Speech-IITM. In signing this licence you confirm that 
you have read and understood the privacy policy and that you consent to the processing of your personal data by 
Speech-IITM staff.

</details>
