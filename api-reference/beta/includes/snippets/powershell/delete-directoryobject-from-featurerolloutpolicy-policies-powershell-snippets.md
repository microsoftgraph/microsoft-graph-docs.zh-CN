---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0f7d8ad37f6a145bdd4d781f30fbb85f4b8a3717
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2022
ms.locfileid: "66445327"
---
```powershell

Import-Module Microsoft.Graph.Identity.SignIns

Remove-MgPolicyFeatureRolloutPolicyApplyToByRef -FeatureRolloutPolicyId $featureRolloutPolicyId -DirectoryObjectId $directoryObjectId

```