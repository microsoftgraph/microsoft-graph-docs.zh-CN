---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4dfbf593a994b80ec252e8625ff5520d7ff417f7
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/16/2019
ms.locfileid: "37544215"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DirectoryObject directoryObject = new DirectoryObject();
directoryObject.Id = "{id}";

graphClient.directoryRoles("{id}").members().references()
    .buildRequest()
    .post(directoryObject);

```