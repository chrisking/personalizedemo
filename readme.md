# Amazon Personalize Workshop

In this workshop you will build your very own recommendation model that will recommend movies to users based on their past preferences. You will further improve the recommendation model to take into account user's interactions with movie items to provide accurate recommendations.  This workshop will use the publicly available movie lens dataset.

## Prerequisites

1. AWS Account
2. User with administrator access to the AWS Account

## Setup

High level steps :

1. Create an S3 bucket that will be used to save movie lens data.
2. Create an IAM policy that provides access to Amazon Personalize APIs.
3. Create an Amazon SageMaker Notebook to explore the movie lens data and use Amazon Personalize APIs to build the recommendation model.

Follow the detailed step-by-step instructions provided in setup.docx

## Agenda

1. `Personalize_BuildCampaign.ipynb`  - Guides you through building your first campaign and recommendation algorithm. 
2. `View_Campaign_And_Interactions.ipynb` - Showcase how to generate a recommendation and how to modify it with real time intent. 
3. `Cleanup.ipynb` - Deletes anything that was created so you are not charged for additional resources.


## Getting Started with Amazon Personalize.

To begin, click `Open Jupyter`, this will take you to the default interface for the Notebook Instance.

Click `New` then click `Terminal`, this will open a BASH shell for you on this instance. 

Enter the following commands to clone this repository onto this instance:

```
cd SageMaker
git clone https://github.com/sirimuppala/personalizedemo.git
```

After that close your Terminal tab and go back to the main Notebook interface.

A new folder titled `personalizedemo` should be visible, click it, click notebooks, then click `Personalize_BuildCampaign.ipynb` this will open the notebook.

If prompted for a kernel, select `conda_python3`.

From here you will follow the instructions outlined in the notebook. 

**Read Every Cell FULLY Before Executing It**

The rest of the lab will take place via the Jupyter notebooks. 

