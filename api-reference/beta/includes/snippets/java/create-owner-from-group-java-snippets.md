---
description: 自动生成的文件。 不修改
ms.openlocfilehash: cdd8cd422dafc3aa99314969961fc4320d06371f
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35858000"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DirectoryObject directoryObject = new DirectoryObject();
directoryObject.additionalDataManager().put("@odata.id", new JsonPrimitive("https://graph.microsoft.com/beta/users/{id}"));

graphClient.groups("{id}").owners().references()
    .buildRequest()
    .post(directoryObject);

```