---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cee7c9c53334f3be1d89502e6924542dafeebf03fda5ee471c407a6f958ed1a1
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57162153"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Todo.Lists["{todoTaskList-id}"]
    .Request()
    .DeleteAsync();

```