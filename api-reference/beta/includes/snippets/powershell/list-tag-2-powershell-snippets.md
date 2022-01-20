---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 398fce2e53de54ab00ddbf3ed947f871fb866429
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62123814"
---
```powershell

Import-Module Microsoft.Graph.Compliance

Get-MgComplianceEdiscoveryCaseTagChildTag -CaseId $caseId -TagId $tagId

```