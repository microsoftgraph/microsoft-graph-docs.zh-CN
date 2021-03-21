---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2b0f43c62e3cb4876a2cf7965c1a67ccfcba7a69
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50963764"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EducationUser educationUser = new EducationUser();
educationUser.additionalDataManager().put("@odata.id", new JsonPrimitive("https://graph.microsoft.com/v1.0/education/users/13015"));

graphClient.education().classes("{class-id}").members().references()
    .buildRequest()
    .post(educationUser);

```