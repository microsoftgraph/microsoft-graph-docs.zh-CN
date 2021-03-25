---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6cfb99329305df9d35592151e8a24e3520bada5d
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/25/2021
ms.locfileid: "51208895"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EducationUser educationUser = new EducationUser();
educationUser.additionalDataManager().put("@odata.id", new JsonPrimitive("https://graph.microsoft.com/v1.0/education/users/13015"));

graphClient.education().classes("{class-id}").members().references()
    .buildRequest()
    .post(educationUser);

```