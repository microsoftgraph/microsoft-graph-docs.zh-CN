---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 957e7660b5001ae3d5d13020ad077c75bd2c2524
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35891058"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DirectoryObject directoryObject = new DirectoryObject();
directoryObject.additionalDataManager().put("@odata.id", new JsonPrimitive("https://graph.microsoft.com/v1.0/directoryObjects/{id}"));

graphClient.directoryRoles("{id}").members().references()
    .buildRequest()
    .post(directoryObject);

```