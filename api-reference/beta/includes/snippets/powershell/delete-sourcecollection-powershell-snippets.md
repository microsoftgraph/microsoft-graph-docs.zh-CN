---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f23102019aed922ac211a6606d51dd4b039d867c
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62103294"
---
```powershell

Import-Module Microsoft.Graph.Compliance

Remove-MgComplianceEdiscoveryCaseSourceCollection -CaseId $caseId -SourceCollectionId $sourceCollectionId

```