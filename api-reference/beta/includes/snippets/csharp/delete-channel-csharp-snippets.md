---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 690db678ce07c8b29957bc91a2d1150dc8ceecf8
ms.sourcegitcommit: 53a57f19a5b16029b540e61ddfba6c2b4e45cfc5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/09/2020
ms.locfileid: "35708713"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Teams["{id}"].Channels["{id}"]
    .Request()
    .DeleteAsync();

```