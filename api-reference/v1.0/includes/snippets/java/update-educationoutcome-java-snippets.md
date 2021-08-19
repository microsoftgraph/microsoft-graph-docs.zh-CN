---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9f3a319222b615ef1e3840dd06c9a40966d342f524b1da586f247de6a1504089
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57278577"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EducationRubricOutcome educationOutcome = new EducationRubricOutcome();
LinkedList<RubricQualityFeedbackModel> rubricQualityFeedbackList = new LinkedList<RubricQualityFeedbackModel>();
RubricQualityFeedbackModel rubricQualityFeedback = new RubricQualityFeedbackModel();
rubricQualityFeedback.qualityId = "9a145aa8-f3d9-43a1-8f77-5387ff0693f2";
EducationItemBody feedback = new EducationItemBody();
feedback.content = "This is feedback specific to the first quality of the rubric.";
feedback.contentType = BodyType.TEXT;
rubricQualityFeedback.feedback = feedback;
rubricQualityFeedbackList.add(rubricQualityFeedback);
RubricQualityFeedbackModel rubricQualityFeedback1 = new RubricQualityFeedbackModel();
rubricQualityFeedback1.qualityId = "d2331fb2-2761-402e-8de6-93e0afaa076e";
EducationItemBody feedback1 = new EducationItemBody();
feedback1.content = "This is feedback specific to the second quality of the rubric.";
feedback1.contentType = BodyType.TEXT;
rubricQualityFeedback1.feedback = feedback1;
rubricQualityFeedbackList.add(rubricQualityFeedback1);
educationOutcome.rubricQualityFeedback = rubricQualityFeedbackList;
LinkedList<RubricQualitySelectedColumnModel> rubricQualitySelectedLevelsList = new LinkedList<RubricQualitySelectedColumnModel>();
RubricQualitySelectedColumnModel rubricQualitySelectedLevels = new RubricQualitySelectedColumnModel();
rubricQualitySelectedLevels.qualityId = "9a145aa8-f3d9-43a1-8f77-5387ff0693f2";
rubricQualitySelectedLevels.columnId = "4fb17a1d-5681-46c2-a295-4e305c3eae23";
rubricQualitySelectedLevelsList.add(rubricQualitySelectedLevels);
RubricQualitySelectedColumnModel rubricQualitySelectedLevels1 = new RubricQualitySelectedColumnModel();
rubricQualitySelectedLevels1.qualityId = "d2331fb2-2761-402e-8de6-93e0afaa076e";
rubricQualitySelectedLevels1.columnId = "aac076bf-51ba-48c5-a2e0-ee235b0b9740";
rubricQualitySelectedLevelsList.add(rubricQualitySelectedLevels1);
educationOutcome.rubricQualitySelectedLevels = rubricQualitySelectedLevelsList;

graphClient.education().classes("acdefc6b-2dc6-4e71-b1e9-6d9810ab1793").assignments("cf6005fc-9e13-44a2-a6ac-a53322006454").submissions("d1bee293-d8bb-48d4-af3e-c8cb0e3c7fe7").outcomes("9c0f2850-ff8f-4fd6-b3ac-e23077b59141")
    .buildRequest()
    .patch(educationOutcome);

```