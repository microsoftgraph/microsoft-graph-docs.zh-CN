---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 98ff120519051e8636142919541ad508f9318d7b6405abe4969155c42b862d74
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57329088"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EducationUser educationUser = new EducationUser();
educationUser.additionalDataManager().put("@odata.id", new JsonPrimitive("https://graph.microsoft.com/v1.0/education/users/14008"));

graphClient.education().schools("{id}").users().references()
    .buildRequest()
    .post(educationUser);

```