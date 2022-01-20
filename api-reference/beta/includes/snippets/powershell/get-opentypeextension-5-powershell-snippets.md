---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a474bd23cd3e1ff8ced1714b9e0b4b88f20557f1
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62112866"
---
```powershell

Import-Module Microsoft.Graph.Mail

Get-MgUserMessage -UserId $userId -Filter "Extensions/any(f:f/id eq 'Com.Contoso.Referral')" -ExpandProperty "Extensions(`$filter=id eq 'Com.Contoso.Referral')" 

```