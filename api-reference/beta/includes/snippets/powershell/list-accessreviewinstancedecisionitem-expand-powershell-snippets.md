---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5039ac4701e6398d90f44f320f8739a5b662e13b
ms.sourcegitcommit: 871db8b3f68489d24e2aeafe694725579ee44c47
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/26/2022
ms.locfileid: "62224914"
---
```powershell

Import-Module Microsoft.Graph.Identity.Governance

Get-MgIdentityGovernanceAccessReviewDecision -AccessReviewInstanceDecisionItemId $accessReviewInstanceDecisionItemId -ExpandProperty "instance(`$expand=definition)" 

```