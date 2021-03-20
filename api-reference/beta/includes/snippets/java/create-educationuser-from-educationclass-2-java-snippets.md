---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d391d4d19fcd174a4a640b79f137c74cd47459e6
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50951522"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EducationUser educationUser = new EducationUser();
educationUser.additionalDataManager().put("@odata.id", new JsonPrimitive("https://graph.microsoft.com/beta/education/users/14011"));

graphClient.education().classes("11017").teachers().references()
    .buildRequest()
    .post(educationUser);

```