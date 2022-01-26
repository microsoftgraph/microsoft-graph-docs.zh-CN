---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 57f85213f7aa39ca13f0a2af572ec2127856b067
ms.sourcegitcommit: 871db8b3f68489d24e2aeafe694725579ee44c47
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/26/2022
ms.locfileid: "62224920"
---
```powershell

Import-Module Microsoft.Graph.Identity.SignIns

Remove-MgIdentityProvider -IdentityProviderId $identityProviderId

```