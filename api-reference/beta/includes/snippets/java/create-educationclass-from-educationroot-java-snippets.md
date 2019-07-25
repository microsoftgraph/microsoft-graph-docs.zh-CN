---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 19de8d5ade1e1bbf130390e8c551c0ac39b24ffd
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35860423"
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