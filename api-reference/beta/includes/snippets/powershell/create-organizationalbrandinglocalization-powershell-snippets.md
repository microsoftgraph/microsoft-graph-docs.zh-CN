---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d538a056f190ebe9ddaa481420dbf091b2f3d45e
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2022
ms.locfileid: "66443291"
---
```powershell

Import-Module Microsoft.Graph.Identity.DirectoryManagement

$params = @{
    BackgroundColor = "#00000F"
    Id = "fr-FR"
    SignInPageText = " "
}

New-MgOrganizationBrandingLocalization -OrganizationId $organizationId -BodyParameter $params

```