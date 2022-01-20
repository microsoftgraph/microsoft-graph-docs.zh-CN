---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d8678d4e1c069db8546701791dc4f2d7f75c5fb1
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62120881"
---
```powershell

Import-Module Microsoft.Graph.Compliance

Get-MgComplianceEdiscoveryCaseLegalHoldUserSource -CaseId $caseId -LegalHoldId $legalHoldId

```