---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4f13909e854cb03cd3cfb0cb522685224dfdd6af
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2022
ms.locfileid: "66502996"
---
```powershell

Import-Module Microsoft.Graph.Identity.SignIns

Remove-MgPolicyMobileDeviceManagementPolicyIncludedGroupByRef -MobilityManagementPolicyId $mobilityManagementPolicyId -GroupId $groupId

```