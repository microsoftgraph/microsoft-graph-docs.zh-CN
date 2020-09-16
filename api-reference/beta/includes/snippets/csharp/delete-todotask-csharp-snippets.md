---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c2a448e03b40faedd27d6bb0131bcd7220c739b2
ms.sourcegitcommit: 7e1993d64cc6d3145ae0ca984fefe74772b6052b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/16/2020
ms.locfileid: "47938442"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Todo.Lists["AAMkADA1MTHgwAAA="].Tasks["721a35e2-35e2-721a-e235-1a72e2351a72"]
    .Request()
    .DeleteAsync();

```