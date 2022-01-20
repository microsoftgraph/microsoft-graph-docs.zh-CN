---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e37794a70defbd2133eebae020a55fcd0be1be5d
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62120104"
---
```powershell

Import-Module Microsoft.Graph.Identity.DirectoryManagement

Remove-MgOrganizationSettingProfileCardProperty -OrganizationId $organizationId -ProfileCardPropertyId $profileCardPropertyId

```