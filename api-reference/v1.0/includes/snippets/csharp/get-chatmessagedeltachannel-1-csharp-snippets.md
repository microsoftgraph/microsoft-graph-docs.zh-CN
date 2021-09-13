---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 562706d355eb64687f13bd9d46b0b72a5acfa139095d856545d0b7cbcad8a4f2
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57221446"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var delta = await graphClient.Teams["{team-id}"].Channels["{channel-id}"].Messages
    .Delta()
    .Request()
    .Top(2)
    .GetAsync();

```