---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5795d1a2249f2585a6ca64e31cfcfbdfaa7d06a8
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62134755"
---
```powershell

Import-Module Microsoft.Graph.Identity.SignIns

Remove-MgPolicyHomeRealmDiscoveryPolicy -HomeRealmDiscoveryPolicyId $homeRealmDiscoveryPolicyId

```