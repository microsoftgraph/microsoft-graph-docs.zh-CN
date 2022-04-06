---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8f6f440a74fb632e24f8e03411bae8a4febfdcac739418da9901d540bbfb7d95
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57219278"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var channels = await graphClient.Teams["{team-id}"].Channels
    .Request()
    .Filter("membershipType eq 'private'")
    .GetAsync();

```