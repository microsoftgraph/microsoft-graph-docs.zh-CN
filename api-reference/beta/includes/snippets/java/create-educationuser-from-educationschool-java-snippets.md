---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3eba9f56ca3ac960e50acb0c9b8d6dc7f215d3f907ff566a8099c7b2b11e1afd
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57106451"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EducationUser educationUser = new EducationUser();
educationUser.additionalDataManager().put("@odata.id", new JsonPrimitive("https://graph.microsoft.com/beta/education/users/14008"));

graphClient.education().schools("{id}").users().references()
    .buildRequest()
    .post(educationUser);

```