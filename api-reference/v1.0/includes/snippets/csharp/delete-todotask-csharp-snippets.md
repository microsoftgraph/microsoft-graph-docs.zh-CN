---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ae81cd94e3fbe7b96b33193b3a35ea714c48ca01b95c2845e77f70a8504ad8b3
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57162946"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Todo.Lists["{todoTaskList-id}"].Tasks["{todoTask-id}"]
    .Request()
    .DeleteAsync();

```