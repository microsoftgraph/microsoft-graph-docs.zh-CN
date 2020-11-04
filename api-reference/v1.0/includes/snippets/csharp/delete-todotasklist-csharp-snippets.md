---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4bb9ff031d7a3abc59fd0748c2aa9f7b1b6f9840
ms.sourcegitcommit: 82da4012294b046416c9ae93d2294d80dab217f6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/04/2020
ms.locfileid: "48904971"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Todo.Lists["AAMkADIyAAAhrbPXAAA="]
    .Request()
    .DeleteAsync();

```