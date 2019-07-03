---
description: 自动生成的文件。 不修改
ms.openlocfilehash: b387746210f47745d74dbab07a4565853e964472
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35467113"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var extension = await graphClient.Me.Messages["AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl==="].Extensions["Com.Contoso.Referral"]
    .Request()
    .GetAsync();

```