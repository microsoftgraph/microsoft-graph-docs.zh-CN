---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9c9fbf500a700719d55f477fbe7704b8c07f4132
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50963406"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var todoTaskList = await graphClient.Me.Todo.Lists["{todoTaskList-id}"]
    .Request()
    .GetAsync();

```