---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 270b9eff397966b4da24112a539bedae5675045a
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/25/2021
ms.locfileid: "51208672"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EducationUser educationUser = new EducationUser();
educationUser.additionalDataManager().put("@odata.id", new JsonPrimitive("https://graph.microsoft.com/beta/education/users/13015"));

graphClient.education().classes("11011").members().references()
    .buildRequest()
    .post(educationUser);

```