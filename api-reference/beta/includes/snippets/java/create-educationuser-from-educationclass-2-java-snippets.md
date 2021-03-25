---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 00509705071c0ff7c0904182d9211cde75c473cf
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/25/2021
ms.locfileid: "51210251"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EducationUser educationUser = new EducationUser();
educationUser.additionalDataManager().put("@odata.id", new JsonPrimitive("https://graph.microsoft.com/beta/education/users/14011"));

graphClient.education().classes("11017").teachers().references()
    .buildRequest()
    .post(educationUser);

```