---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 296a3c75c7d26efb569e47cfb1d9405b483943bc
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65212520"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var allChannels = await graphClient.Teams["{team-id}"].AllChannels
    .Request()
    .GetAsync();

```