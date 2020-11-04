---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ba6dc841a49c706614033d8ccbaa31491dfcea2d
ms.sourcegitcommit: 82da4012294b046416c9ae93d2294d80dab217f6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/04/2020
ms.locfileid: "48903826"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var tasks = await graphClient.Me.Todo.Lists["35e2-35e2-721a-e235-1a72e2351a7"].Tasks
    .Request()
    .GetAsync();

```