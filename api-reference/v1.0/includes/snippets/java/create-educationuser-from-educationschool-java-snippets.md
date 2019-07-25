---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 3c71e1f2842b9e80db22b5216f1257fdba3f548f
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35887637"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EducationUser educationUser = new EducationUser();
educationUser.additionalDataManager().put("@odata.id", new JsonPrimitive("https://graph.microsoft.com/v1.0/education/users/14008"));

graphClient.education().schools("{id}").users().references()
    .buildRequest()
    .post(educationUser);

```