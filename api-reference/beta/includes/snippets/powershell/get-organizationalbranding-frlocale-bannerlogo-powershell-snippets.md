---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f1fe26c4302e23a88c84a4a7db1bf27ecfb347b9
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2022
ms.locfileid: "66440605"
---
```powershell

Import-Module Microsoft.Graph.Identity.DirectoryManagement

Get-MgOrganizationBrandingLocalizationBannerLogo -OrganizationId $organizationId -OrganizationalBrandingLocalizationId $organizationalBrandingLocalizationId

```