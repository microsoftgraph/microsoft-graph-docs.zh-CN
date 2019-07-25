---
description: 自动生成的文件。 不修改
ms.openlocfilehash: d5a410f45520840b68c291a6ca72748015c1d0c0
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35721252"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var extension = await graphClient.Me.Messages["AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl==='"].Extensions["Com.Contoso.Referral"]
    .Request()
    .GetAsync();

```