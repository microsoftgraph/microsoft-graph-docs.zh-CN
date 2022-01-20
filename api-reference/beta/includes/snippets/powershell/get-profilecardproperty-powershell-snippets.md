---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e81bdfeef1d18f37f25c800e7f6c661f3dcb224e
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62132760"
---
```powershell

Import-Module Microsoft.Graph.Identity.DirectoryManagement

Get-MgOrganizationSettingProfileCardProperty -OrganizationId $organizationId -ProfileCardPropertyId $profileCardPropertyId

```