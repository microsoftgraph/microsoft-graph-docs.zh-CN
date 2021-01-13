---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 58a156ba3f50603201acd6e5c9e16df22a17654d
ms.sourcegitcommit: a9731e19589dcb5c0c6fe2e24b008c86573ef803
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/13/2021
ms.locfileid: "49844486"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var identityApiConnector = await graphClient.Identity.ApiConnectors["{id}"]
    .Request()
    .GetAsync();

```