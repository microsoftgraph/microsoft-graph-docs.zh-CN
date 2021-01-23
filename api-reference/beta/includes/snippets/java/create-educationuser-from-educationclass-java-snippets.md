---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f80bc0523e1c68bd8e61cf2dbb8ad9843e638684
ms.sourcegitcommit: 9a5facff47a8d4e05ecd2c6cd68294a948c47c4d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2021
ms.locfileid: "49945194"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EducationUser educationUser = new EducationUser();
educationUser.additionalDataManager().put("@odata.id", new JsonPrimitive("https://graph.microsoft.com/beta/education/users/13015"));

graphClient.education().classes("11011").members().references()
    .buildRequest()
    .post(educationUser);

```