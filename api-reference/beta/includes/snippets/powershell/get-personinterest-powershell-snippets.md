---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ea00fbc90f5e36fba5717dcf10eaf66d0fb46b30
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62118641"
---
```powershell

Import-Module Microsoft.Graph.People

Get-MgUserProfileInterest -UserId $userId -PersonInterestId $personInterestId

```