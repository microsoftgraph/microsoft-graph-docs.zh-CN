---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4dee30236be84fcae498691b64355246751fcbd155716de513c4bc9f49f928a9
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57277530"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EducationUser educationUser = new EducationUser();
educationUser.additionalDataManager().put("@odata.id", new JsonPrimitive("https://graph.microsoft.com/v1.0/education/users/13015"));

graphClient.education().classes("{class-id}").members().references()
    .buildRequest()
    .post(educationUser);

```