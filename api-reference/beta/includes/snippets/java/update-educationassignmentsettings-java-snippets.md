---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 46e3c5d3297773a0e503910377cd09a0589c0fb3
ms.sourcegitcommit: 69c355eeb620b76ca70d896f984e21c32ac09eb0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2021
ms.locfileid: "50092494"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EducationAssignmentSettings educationAssignmentSettings = new EducationAssignmentSettings();
educationAssignmentSettings.submissionAnimationDisabled = true;

graphClient.education().classes("{id}").assignmentSettings()
    .buildRequest()
    .patch(educationAssignmentSettings);

```