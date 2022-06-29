---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d20816d76681c565794557837638e6204456b462
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2022
ms.locfileid: "66436578"
---
```powershell

Import-Module Microsoft.Graph.Identity.SignIns

Get-MgOrganizationCertificateBasedAuthConfiguration -OrganizationId $organizationId -CertificateBasedAuthConfigurationId $certificateBasedAuthConfigurationId

```