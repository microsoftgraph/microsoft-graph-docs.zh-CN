---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4e9402850099aa344030a6548c138a2690141fa24436a0ff5805f2751e4f75ac
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57164182"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Activities["{userActivity-id}"]
    .Request()
    .DeleteAsync();

```