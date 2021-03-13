---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a1f69c52e8151c21057280633463a77f8daf6e8e
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50781525"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var identityApiConnector = await graphClient.Identity.ApiConnectors["{identityApiConnector-id}"]
    .Request()
    .GetAsync();

```