---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f3935e4d1f823cb9290cd6629592e2c60d77c73f
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/25/2021
ms.locfileid: "51208835"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EducationClass educationClass = new EducationClass();
educationClass.additionalDataManager().put("@odata.id", new JsonPrimitive("https://graph.microsoft.com/v1.0/education/classes/11006"));

graphClient.education().schools("{school-id}").classes().references()
    .buildRequest()
    .post(educationClass);

```