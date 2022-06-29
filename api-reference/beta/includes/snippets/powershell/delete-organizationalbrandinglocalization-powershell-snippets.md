---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0cf831078dfd03fd79fb699bdefc0e2bb11341b2
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2022
ms.locfileid: "66438984"
---
```powershell

Import-Module Microsoft.Graph.Identity.DirectoryManagement

Remove-MgOrganizationBrandingLocalization -OrganizationId $organizationId -OrganizationalBrandingLocalizationId $organizationalBrandingLocalizationId

```