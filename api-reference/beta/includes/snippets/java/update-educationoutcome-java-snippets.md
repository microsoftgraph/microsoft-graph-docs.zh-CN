---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 85ffb3dc6e122f47c7147542c178cf05d109c42c3bf19cd69d97c4a333042176
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57163435"
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

graphClient.education().classes("{id}").assignments("{id}").submissions("{id}").outcomes("{id}")
    .buildRequest()
    .patch(educationOutcome);

```