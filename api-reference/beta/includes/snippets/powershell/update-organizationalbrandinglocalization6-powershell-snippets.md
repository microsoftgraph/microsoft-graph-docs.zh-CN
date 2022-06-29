---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0c7fe258d60a414dccad7cb1aeea812a6c7a5af3
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2022
ms.locfileid: "66443306"
---
```powershell

Import-Module Microsoft.Graph.Identity.DirectoryManagement

$params = @{
    BackgroundColor = "#00000F"
    SignInPageText = "Welcome to Contoso France"
}

Update-MgOrganizationBrandingLocalization -OrganizationId $organizationId -OrganizationalBrandingLocalizationId $organizationalBrandingLocalizationId -BodyParameter $params

```