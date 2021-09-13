---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0e2057098f50ead4a40719d3135f4fbffa53c98116b4fae8b4c59a08b1f713a2
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57333158"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var delta = await graphClient.Teams["{team-id}"].Channels["{channel-id}"].Messages
    .Delta()
    .Request()
    .GetAsync();

```