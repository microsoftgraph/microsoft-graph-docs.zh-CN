---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2e46a4fe395ab343acc734b7330629e4d80a31f0141b97f96c6e2515b80e70c7
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57279508"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var lists = await graphClient.Me.Todo.Lists
    .Request()
    .GetAsync();

```