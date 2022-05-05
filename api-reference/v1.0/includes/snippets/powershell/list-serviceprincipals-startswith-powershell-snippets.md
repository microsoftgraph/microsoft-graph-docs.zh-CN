---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f976214e87a88cc392ab37ac182680115a9ee4f7
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65203095"
---
```powershell

Import-Module Microsoft.Graph.Applications

Get-MgServicePrincipal -Filter "startswith(displayName, 'a')" -CountVariable CountVar -Top 1 -Sort "displayName" -ConsistencyLevel eventual 


```