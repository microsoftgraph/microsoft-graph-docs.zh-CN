---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 31020ecc5f4e784b5182c4f7453c588567ce78c5
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62135518"
---
```powershell

Import-Module Microsoft.Graph.Search

$params = @{
    Name = "Contoso HR Service Tickets"
    Description = "Connection to index HR service tickets"
}

Update-MgExternalConnection -ExternalConnectionId $externalConnectionId -BodyParameter $params

```