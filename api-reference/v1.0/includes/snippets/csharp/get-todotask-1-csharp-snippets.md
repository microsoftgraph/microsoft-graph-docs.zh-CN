---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2b2a322bfdab2ab81bcc7dd68748244f40ed306ce9c0972739bd6f3abb0deb5c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57162317"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var todoTask = await graphClient.Me.Todo.Lists["{todoTaskList-id}"].Tasks["{todoTask-id}"]
    .Request()
    .GetAsync();

```