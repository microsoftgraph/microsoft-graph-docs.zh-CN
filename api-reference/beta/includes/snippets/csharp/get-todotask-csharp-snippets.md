---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ba6dc841a49c706614033d8ccbaa31491dfcea2d
ms.sourcegitcommit: 7e1993d64cc6d3145ae0ca984fefe74772b6052b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/16/2020
ms.locfileid: "47938472"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var tasks = await graphClient.Me.Todo.Lists["35e2-35e2-721a-e235-1a72e2351a7"].Tasks
    .Request()
    .GetAsync();

```