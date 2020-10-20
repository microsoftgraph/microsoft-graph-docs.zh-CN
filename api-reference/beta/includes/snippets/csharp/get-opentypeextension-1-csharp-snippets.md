---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d5a410f45520840b68c291a6ca72748015c1d0c0
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48621258"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var extension = await graphClient.Me.Messages["AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl==='"].Extensions["Com.Contoso.Referral"]
    .Request()
    .GetAsync();

```