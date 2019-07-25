---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 5fec814ecf6419fe51b0e1356fbe5e239493b0ba
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35858086"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DirectoryObject directoryObject = new DirectoryObject();
directoryObject.additionalDataManager().put("@odata.id", new JsonPrimitive("https://graph.microsoft.com/beta/directoryObjects/{id}"));

graphClient.groups("{id}").members().references()
    .buildRequest()
    .post(directoryObject);

```