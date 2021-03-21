---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: dbeea9d2d2facf4478abcef3bb8af88607420b23
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50978612"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EducationUser educationUser = new EducationUser();
educationUser.additionalDataManager().put("@odata.id", new JsonPrimitive("https://graph.microsoft.com/v1.0/education/users/14008"));

graphClient.education().schools("{id}").users().references()
    .buildRequest()
    .post(educationUser);

```