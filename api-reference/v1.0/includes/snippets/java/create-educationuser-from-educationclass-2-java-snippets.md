---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 51cd9c58d79164012b58bf44ea67d8a6a006af31a8169fd5d3c5f588ffaced9d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57409568"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EducationUser educationUser = new EducationUser();
educationUser.additionalDataManager().put("@odata.id", new JsonPrimitive("https://graph.microsoft.com/v1.0/education/users/14011"));

graphClient.education().classes("{class-id}").teachers().references()
    .buildRequest()
    .post(educationUser);

```