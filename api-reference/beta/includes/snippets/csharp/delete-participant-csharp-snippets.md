---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f827b1490e101fd366270f87bfc26b85f89bf2ab
ms.sourcegitcommit: a3fc420a5639c0f4e89af2b602db17392e176802
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/23/2020
ms.locfileid: "48222888"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Communications.Calls["{id}"].Participants["{id}"]
    .Request()
    .DeleteAsync();

```