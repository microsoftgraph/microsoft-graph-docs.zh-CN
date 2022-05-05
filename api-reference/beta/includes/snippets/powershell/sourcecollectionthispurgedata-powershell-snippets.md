---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d5cbbd2e05a6e16e71a0b419343bb399d8fd7709
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65211429"
---
```powershell

Import-Module Microsoft.Graph.Compliance

Clear-MgComplianceEdiscoveryCaseSourceCollectionData -CaseId $caseId -SourceCollectionId $sourceCollectionId

```