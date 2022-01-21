---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cd21700978b1e3dc699a073f614cf827331ec9eb
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62118865"
---
```powershell

Import-Module Microsoft.Graph.Identity.SignIns

Get-MgPolicyFeatureRolloutPolicy -FeatureRolloutPolicyId $featureRolloutPolicyId -ExpandProperty "appliesTo" 

```