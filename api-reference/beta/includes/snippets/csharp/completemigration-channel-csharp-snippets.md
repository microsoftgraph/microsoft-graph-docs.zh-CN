---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1f24379009fb1c9ab62760faa70eaa2d096b3ca2
ms.sourcegitcommit: 82da4012294b046416c9ae93d2294d80dab217f6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/04/2020
ms.locfileid: "48903969"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Teams["{teamId}"].Channels["{channelId}"]
    .CompleteMigration()
    .Request()
    .PostAsync();

```