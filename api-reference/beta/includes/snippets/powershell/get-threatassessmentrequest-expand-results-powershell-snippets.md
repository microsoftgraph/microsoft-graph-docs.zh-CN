---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fd800f92852481ffccd85af67c70aab3806e5a2e
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62115614"
---
```powershell

Import-Module Microsoft.Graph.Identity.SignIns

Get-MgInformationProtectionThreatAssessmentRequest -ThreatAssessmentRequestId $threatAssessmentRequestId -ExpandProperty "results" 

```