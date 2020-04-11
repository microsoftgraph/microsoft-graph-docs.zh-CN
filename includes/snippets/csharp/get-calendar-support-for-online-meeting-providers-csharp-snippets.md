---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4692306cd41c8a719334c5e844bf47b00b98cc4c
ms.sourcegitcommit: fce7ce328f0c88c6310af9cc85d12bcebc88a6c3
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/28/2019
ms.locfileid: "39636965"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var calendar = await graphClient.Me.Calendar
    .Request()
    .GetAsync();

```