---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f976214e87a88cc392ab37ac182680115a9ee4f7
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62112775"
---
```powershell

Import-Module Microsoft.Graph.Applications

Get-MgServicePrincipal -Filter "startswith(displayName, 'a')" -CountVariable CountVar -Top 1 -Sort "displayName" -ConsistencyLevel eventual 


```