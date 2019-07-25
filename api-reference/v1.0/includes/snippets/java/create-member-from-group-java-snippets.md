---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c832b0b6b98d051e30334b104883f87a8b9ce27d
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35890074"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DirectoryObject directoryObject = new DirectoryObject();
directoryObject.additionalDataManager().put("@odata.id", new JsonPrimitive("https://graph.microsoft.com/v1.0/directoryObjects/{id}"));

graphClient.groups("{id}").members().references()
    .buildRequest()
    .post(directoryObject);

```