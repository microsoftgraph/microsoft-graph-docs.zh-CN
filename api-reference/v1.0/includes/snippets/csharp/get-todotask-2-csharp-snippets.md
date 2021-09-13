---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5e76da6ede90066d7daec46bedf390ae2fb4a4641c68efdb6b4b6466005d5443
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57279644"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var tasks = await graphClient.Me.Todo.Lists["{todoTaskList-id}"].Tasks
    .Request()
    .GetAsync();

```