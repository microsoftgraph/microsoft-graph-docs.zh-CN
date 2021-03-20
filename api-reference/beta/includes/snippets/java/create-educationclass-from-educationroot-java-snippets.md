---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 03e4e1f26596968a2c067ffd604855ad4740c5cc
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50977490"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

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