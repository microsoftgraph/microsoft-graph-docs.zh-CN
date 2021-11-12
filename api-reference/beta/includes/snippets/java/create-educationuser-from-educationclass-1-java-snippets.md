---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9bcf6d1d29a9e51c89356c14077c42283a3e796db8cb3cc4631453b6b4529869
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57220692"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EducationUser educationUser = new EducationUser();
educationUser.additionalDataManager().put("@odata.id", new JsonPrimitive("https://graph.microsoft.com/beta/education/users/13015"));

graphClient.education().classes("11011").members().references()
    .buildRequest()
    .post(educationUser);

```