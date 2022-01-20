---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ccf51036c59abd5ca0b823693dd403c6056fcb03
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62100493"
---
```powershell

Import-Module Microsoft.Graph.Identity.SignIns

Remove-MgPolicyClaimMappingPolicy -ClaimsMappingPolicyId $claimsMappingPolicyId

```