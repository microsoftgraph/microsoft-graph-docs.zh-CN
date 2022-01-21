---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 57e72efedabb0272ad427409e10437f207cc56fb
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62126641"
---
```powershell

Import-Module Microsoft.Graph.Users

Get-MgUser -Filter "startswith(displayName,'Eric')" -Property "displayName,signInActivity" 

```