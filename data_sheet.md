# Datasheet Template

## Motivation

**For what purpose was the dataset created?** 
The original dataset was created for classifying user feedback in English and Italian into problem reports, inquiries, and irrelevant.
The labelled dataset was created for classifying user feedback in English into Kano model factors.

**Who created the dataset (e.g., which team, research group) and on behalf of which entity (e.g., company, institution, organization)? Who funded the creation of the dataset?**
The original dataset was created by Stanik, Haering and Maalej for the 27th International Requirements Engineering Conference Workshops (REW).
This was then used and relabelled by Binder, Vogt, Bajraktari and Vogelsang or the University of Cologne.

It's unclear who funded the creation of the datasets.
 
## Composition

**What do the instances that comprise the dataset represent (e.g., documents, photos, people, countries)?**
Each instance in the dataset is an individual review left for an app on either the App Store or Google Play Store.

**How many instances of each type are there?**
There are 6070 instances in the dataset.

**Is there any missing data?**
There is no missing data.

**Does the dataset contain data that might be considered confidential (e.g., data that is protected by legal privilege or by    doctor–patient confidentiality, data that includes the content of individuals’ non-public communications)?**
The dataset may contain PII accidentally left by the reviewer in the review text. There are no other fields that may contain PII.

## Collection process

**How was the data acquired?**
The collection process for the original data is unavailable as the paper is behind a paywall at: https://ieeexplore.ieee.org/document/8933719

**If the data is a sample of a larger subset, what was the sampling strategy?**
The original set of collected reviews was filtered to only filtering out reviews which were not written in English, or reviews containing only characters and no words.

**Over what time frame was the data collected?**
Unsure as the paper is behind a paywall.

## Preprocessing/cleaning/labelling

**Was any preprocessing/cleaning/labeling of the data done (e.g., discretization or bucketing, tokenization, part-of-speech tagging, SIFT feature extraction, removal of instances, processing of missing values)? If so, please provide a description. If not, you may skip the remaining questions in this section.**
The original set of collected reviews was filtered to only filtering out reviews which were not written in English, or reviews containing only characters and no words.
The data was then labelled according to the Kano model, considering only the review text, and no further context on the app.
Each review was only assigned one label, even if the review mentions multiple features. If multiple features are mentioned in the review, the feature that was most prominent was used for labelling.
The labelling was done by two independent researchers, with a tie break labeler where ther was disagreement between the two labellers.

The guidelines for reviewing were as below:

```
Basic
– user discontinues using the app or switches to alternative
– app is not usable (e.g., crashes, log in not possible)
– lack of a basic feature results in a bad rating

Delighter
– app is favored and recommended over similar apps due to these features
– user is a long term user due to these features
– praise or suggestion for addition

Performance
– moderate amount of expressed joy / annoyance
– constructive criticism / suggestions

Irrelevant
– cannot be labeled as any other category
– no clear reference to a distinct feature
```

**Was the “raw” data saved in addition to the preprocessed/cleaned/labeled data (e.g., to support unanticipated future uses)?**
The raw data is not available.

## Uses

**What other tasks could the dataset be used for?**
The dataset could be used to supplement other exisitng datasets on app reviews.
This could be used for out of sample testing of other models built to classify or cluster reviews.

**Is there anything about the composition of the dataset or the way it was collected and preprocessed/cleaned/labeled that might impact future uses? For example, is there anything that a dataset consumer might need to know to avoid uses that could result in unfair treatment of individuals or groups (e.g., stereotyping, quality of service issues) or other risks or harms (e.g., legal risks, financial harms)? If so, please provide a description. Is there anything a dataset consumer could do to mitigate these risks or harms?**
The dataset might contain PII accidentally revealed by the reviewr in their review.

**Are there tasks for which the dataset should not be used? If so, please provide a description.**
The dataset might not be sufficient for creating generic models for categorising app reviews.

## Distribution

**How has the dataset already been distributed?** 
The dataset is available at this link: https://figshare.com/articles/dataset/Automatically_Classifying_Kano_Model_Factors_in_App_Reviews/21618858 

**Is it subject to any copyright or other intellectual property (IP) license, and/or under applicable terms of use (ToU)?** 
The dataset is publically available.

## Maintenance
This dataset is not maintained.

