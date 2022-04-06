---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4924133a5ee1c02e9fd4e715a89bb54311d084ff
ms.sourcegitcommit: 0bcc0a93f37db6013be40dc8d36717aeeeef7fb6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/16/2022
ms.locfileid: "63516245"
---
```powershell

Import-Module Microsoft.Graph.Identity.Governance

Get-MgIdentityGovernanceTermOfUseAgreement -AgreementId $agreementId -ExpandProperty "files" 

```