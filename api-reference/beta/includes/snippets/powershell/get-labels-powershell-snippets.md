---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0c84331c25fabd6f33b3c4abbd7c8ea5572ab7e8
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2022
ms.locfileid: "66439598"
---
```powershell

Import-Module Microsoft.Graph.Identity.SignIns

# A UPN can also be used as -UserId.
Get-MgUserInformationProtectionPolicyLabel -UserId $userId

```