---
description: 自动生成的文件。 不修改
ms.openlocfilehash: d391d4d19fcd174a4a640b79f137c74cd47459e6
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35860537"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EducationUser educationUser = new EducationUser();
educationUser.additionalDataManager().put("@odata.id", new JsonPrimitive("https://graph.microsoft.com/beta/education/users/14011"));

graphClient.education().classes("11017").teachers().references()
    .buildRequest()
    .post(educationUser);

```