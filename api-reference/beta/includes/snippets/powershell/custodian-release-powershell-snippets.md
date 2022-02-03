---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2e279e68fcf35aa627467552aa359ddb6acf8816
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62343528"
---
```powershell

Import-Module Microsoft.Graph.Compliance

Publish-MgComplianceEdiscoveryCaseCustodian -CaseId $caseId -CustodianId $custodianId

```