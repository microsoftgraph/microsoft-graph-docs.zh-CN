---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 965f174e0a07849275a5a64b3d5fefc9b68aa0cf
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "40865843"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var reason = RejectReason.None;

await graphClient.Communications.Calls["57dab8b1-894c-409a-b240-bd8beae78896"]
    .Reject(reason,null)
    .Request()
    .PostAsync();

```