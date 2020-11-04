---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bbf82e298956f8322b01a2d9967096f779d3ae76
ms.sourcegitcommit: 82da4012294b046416c9ae93d2294d80dab217f6
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/04/2020
ms.locfileid: "48905016"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var chatMessage = await graphClient.Teams["{id}"].Channels["{id}"].Messages["delta"]
    .Request()
    .GetAsync();

```