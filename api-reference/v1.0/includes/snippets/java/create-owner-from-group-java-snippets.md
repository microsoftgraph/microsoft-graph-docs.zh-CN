---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cabd0b55e37ab97c057640301701281f23f42148
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35884747"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DirectoryObject directoryObject = new DirectoryObject();
directoryObject.additionalDataManager().put("@odata.id", new JsonPrimitive("https://graph.microsoft.com/v1.0/users/{id}"));

graphClient.groups("{id}").owners().references()
    .buildRequest()
    .post(directoryObject);

```