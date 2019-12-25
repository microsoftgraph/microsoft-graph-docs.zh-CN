---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 08985efe8694ce4246e090a1ac844e0189432718
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "40865859"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Communications.Calls["2e1a0b00-2db4-4022-9570-243709c565ab"]
    .KeepAlive()
    .Request()
    .PostAsync();

```