---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 37fcdaa5730c6dc083b605573fa0df95e0e89c5a
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/16/2019
ms.locfileid: "37544216"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DirectoryObject directoryObject = new DirectoryObject();
directoryObject.Id = "{id}";

graphClient.groups("{id}").owners().references()
    .buildRequest()
    .post(directoryObject);

```