---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f237adfe14f33a24d8c089165568f65543000148
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/16/2019
ms.locfileid: "37544225"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DirectoryObject directoryObject = new DirectoryObject();
directoryObject.Id = "{id}";

graphClient.groups("{id}").members().references()
    .buildRequest()
    .post(directoryObject);

```