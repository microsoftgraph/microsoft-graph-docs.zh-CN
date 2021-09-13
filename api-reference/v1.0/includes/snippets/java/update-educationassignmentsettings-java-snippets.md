---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8aaee210f269d0eb32fb2f5ae768f685c62f08d41b1dd11ca339bafe203fa467
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57277536"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EducationAssignmentSettings educationAssignmentSettings = new EducationAssignmentSettings();
educationAssignmentSettings.submissionAnimationDisabled = true;

graphClient.education().classes("acdefc6b-2dc6-4e71-b1e9-6d9810ab1793").assignmentSettings()
    .buildRequest()
    .patch(educationAssignmentSettings);

```