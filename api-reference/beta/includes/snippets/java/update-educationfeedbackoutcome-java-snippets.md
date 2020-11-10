---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b84b689be9a86934f86ad706e913b7e561a9dc3c
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48966136"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EducationFeedbackOutcome educationOutcome = new EducationFeedbackOutcome();
EducationFeedback feedback = new EducationFeedback();
EducationItemBody text = new EducationItemBody();
text.content = "This is feedback for the assignment as a whole.";
text.contentType = BodyType.TEXT;
feedback.text = text;
educationOutcome.feedback = feedback;

graphClient.education().me().assignments("{id}").submissions("{id}").outcomes("{id}")
    .buildRequest()
    .patch(educationOutcome);

```