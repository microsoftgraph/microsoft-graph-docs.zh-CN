---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 040c8a0dfc0bfdc45f6ff4b2ec241d66dab1ae49
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63332735"
---
```powershell

Import-Module Microsoft.Graph.Identity.Governance

Remove-MgIdentityGovernanceTermOfUseAgreement -AgreementId $agreementId

```