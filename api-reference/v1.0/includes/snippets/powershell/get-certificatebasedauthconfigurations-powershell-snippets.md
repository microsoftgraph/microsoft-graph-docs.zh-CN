---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 360896b932983d8f04d76d33740188393dbc1992
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62129141"
---
```powershell

Import-Module Microsoft.Graph.Identity.SignIns

Get-MgOrganizationCertificateBasedAuthConfiguration -OrganizationId $organizationId

```