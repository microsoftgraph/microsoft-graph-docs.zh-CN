---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d04e503f4ac9903ae8a061eefddf7ea11f02cda3
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62133796"
---
```powershell

Import-Module Microsoft.Graph.Compliance

Get-MgComplianceEdiscoveryCaseSourceCollectionAdditionalSource -CaseId $caseId -SourceCollectionId $sourceCollectionId

```