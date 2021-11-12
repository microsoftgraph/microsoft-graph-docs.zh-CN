---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3dc4702a2523154a737207907cee64842bc4a8fa70451691e442e6896342fd16
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57219767"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EducationAssignmentSettings educationAssignmentSettings = new EducationAssignmentSettings();
educationAssignmentSettings.submissionAnimationDisabled = true;

graphClient.education().classes("{id}").assignmentSettings()
    .buildRequest()
    .patch(educationAssignmentSettings);

```