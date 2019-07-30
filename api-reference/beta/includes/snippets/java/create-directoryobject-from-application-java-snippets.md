---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 8487f344990ce55e11b7b9808eaa6bd4fa2d43b9
ms.sourcegitcommit: 56c0b609dfb1bc5d900956f407d107cdab7086e8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/30/2019
ms.locfileid: "35930436"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DirectoryObject directoryObject = new DirectoryObject();
directoryObject.additionalDataManager().put("@odata.id", new JsonPrimitive("https://graph.microsoft.com/beta/directoryObjects/{id}"));

graphClient.applications("{id}").owners().references()
    .buildRequest()
    .post(directoryObject);

```