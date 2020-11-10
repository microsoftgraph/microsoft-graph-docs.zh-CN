---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 19de8d5ade1e1bbf130390e8c551c0ac39b24ffd
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48966064"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EducationClass educationClass = new EducationClass();
educationClass.description = "Health Level 1";
educationClass.classCode = "Health 501";
educationClass.displayName = "Health 1";
educationClass.externalId = "11019";
educationClass.externalName = "Health Level 1";
educationClass.externalSource = EducationExternalSource.SIS;
educationClass.mailNickname = "fineartschool.net";

graphClient.education().classes()
    .buildRequest()
    .post(educationClass);

```