---
description: 自动生成的文件。 不修改
ms.openlocfilehash: f43544294585dd7f6eaaab7a443c14ea9469b8b9
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35866820"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DirectoryObject directoryObject = new DirectoryObject();
directoryObject.additionalDataManager().put("@odata.id", new JsonPrimitive("https://graph.microsoft.com/v1.0/users/{id}"));

graphClient.users("{id}").manager().reference()
    .buildRequest()
    .put(directoryObject);

```