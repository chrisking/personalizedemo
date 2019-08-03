# Amazon Personalize Workshop

In this workshop you will build your very own recommendation model that will recommend movies to users based on their past preferences. You will further improve the recommendation model to take into account user's interactions with movie items to provide accurate recommendations.  This workshop will use the publicly available movie lens dataset.

## Prerequisites

1. AWS Account
2. User with administrator access to the AWS Account

## Process

1. First you will deploy a CloudFormation template that will do the following:
 1. Create an S3 bucket for all of your data storage.
 1. Create a SageMaker Notebook Instance for you to complete the workshop.
 1. Create the IAM policies needed for your notebook.
 1. Clone this repository into the notebook so you are ready to work.
1. Open the notebook and follow the instructions below.

## Building Your Environment

As mentioned above, the first step is to deploy a CloudFormation template that will perform much of the initial setup for you. In another browser window login to your AWS account. Once you have done that click the link below to start the process of deploying the items you need via CloudFormation.

[![Launch Stack](https://s3.amazonaws.com/cloudformation-examples/cloudformation-launch-stack.png)](https://console.aws.amazon.com/cloudformation/home#/stacks/new?stackName=PersonalizeDemo&templateURL=https://raw.githubusercontent.com/chrisking/personalizedemo/cloudformation/PersonalizeDemo.yaml)

The default options should suffice but you will need to change the S3 bucket name to reflect your name. Do not use special characters, uppercase characters, and it must be a unique value. If it fails to create a bucket simply try something more complex in your next attempt.


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

