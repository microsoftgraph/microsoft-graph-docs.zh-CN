---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1958306968c6464c15f7341231994166ba30b6cb
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2022
ms.locfileid: "66438722"
---
```powershell

Import-Module Microsoft.Graph.Security

Remove-MgSecurityCaseEdiscoveryCaseLegalHold -EdiscoveryCaseId $ediscoveryCaseId -EdiscoveryHoldPolicyId $ediscoveryHoldPolicyId

```