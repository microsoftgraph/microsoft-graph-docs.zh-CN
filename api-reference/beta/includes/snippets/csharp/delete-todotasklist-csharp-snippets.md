---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4bb9ff031d7a3abc59fd0748c2aa9f7b1b6f9840
ms.sourcegitcommit: 7e1993d64cc6d3145ae0ca984fefe74772b6052b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/16/2020
ms.locfileid: "47938453"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Todo.Lists["AAMkADIyAAAhrbPXAAA="]
    .Request()
    .DeleteAsync();

```