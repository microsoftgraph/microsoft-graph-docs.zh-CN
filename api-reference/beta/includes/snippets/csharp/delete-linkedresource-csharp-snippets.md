---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 895361e682602ff9de07fe85f16002054811deed954f5a47e8a17c62436912c1
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57220655"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Todo.Lists["{todoTaskList-id}"].Tasks["{todoTask-id}"].LinkedResources["{linkedResource-id}"]
    .Request()
    .DeleteAsync();

```