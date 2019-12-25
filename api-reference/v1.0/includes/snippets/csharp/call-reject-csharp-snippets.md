---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6b9bd055a7a3f654bb73f7fa5bd942fe24145abb
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "40865836"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var reason = RejectReason.Busy;

await graphClient.Communications.Calls["57dab8b1-894c-409a-b240-bd8beae78896"]
    .Reject(reason,null)
    .Request()
    .PostAsync();

```