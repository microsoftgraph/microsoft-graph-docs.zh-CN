---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0a258796262ad88407d04bf9a908a4cbc88ad4f4
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/25/2021
ms.locfileid: "51208612"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EducationUser educationUser = new EducationUser();
educationUser.additionalDataManager().put("@odata.id", new JsonPrimitive("https://graph.microsoft.com/v1.0/education/users/14011"));

graphClient.education().classes("{class-id}").teachers().references()
    .buildRequest()
    .post(educationUser);

```