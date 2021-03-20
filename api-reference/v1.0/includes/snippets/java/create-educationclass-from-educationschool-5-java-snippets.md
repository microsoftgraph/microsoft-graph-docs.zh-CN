---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: de9887678d93b1198cff78eeb7f853cb96ff6fe7
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50953654"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EducationClass educationClass = new EducationClass();
educationClass.additionalDataManager().put("@odata.id", new JsonPrimitive("https://graph.microsoft.com/v1.0/education/classes/11006"));

graphClient.education().schools("{school-id}").classes().references()
    .buildRequest()
    .post(educationClass);

```