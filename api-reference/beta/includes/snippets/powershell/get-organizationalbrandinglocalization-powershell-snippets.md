---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0522532031bac25070e800eae6940e3d03243156
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2022
ms.locfileid: "66446413"
---
```powershell

Import-Module Microsoft.Graph.Identity.DirectoryManagement

Get-MgOrganizationBrandingLocalization -OrganizationId $organizationId -OrganizationalBrandingLocalizationId $organizationalBrandingLocalizationId

```