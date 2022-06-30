---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0ee99498648d8e1c67182966b3966e5f1e2863dd
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2022
ms.locfileid: "66443307"
---
```powershell

Import-Module Microsoft.Graph.Identity.DirectoryManagement

$params = @{
    SignInPageText = "Welcome to Contoso France."
    UsernameHintText = " "
}

Update-MgOrganizationBrandingLocalization -OrganizationId $organizationId -OrganizationalBrandingLocalizationId $organizationalBrandingLocalizationId -BodyParameter $params

```