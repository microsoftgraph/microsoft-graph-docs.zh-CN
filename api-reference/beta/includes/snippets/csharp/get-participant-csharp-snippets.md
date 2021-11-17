---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 76e303fc3ca9c3803ed404fd76549e900433c4da7e247fefd4166ade1d648497
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57329014"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var participant = await graphClient.Communications.Calls["{call-id}"].Participants["{participant-id}"]
    .Request()
    .GetAsync();

```