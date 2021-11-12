---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 42f4b4300ba58eea39ff89517c5ad345158b1fbc29743c9ae4f43fded7b0550e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104408"
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