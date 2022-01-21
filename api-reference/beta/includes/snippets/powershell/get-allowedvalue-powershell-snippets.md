---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 91470253ebbbcd945a402eb3d53d216c2fef4e90
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62103931"
---
```powershell

Import-Module Microsoft.Graph.Identity.DirectoryManagement

Get-MgDirectoryCustomSecurityAttributeDefinitionAllowedValue -CustomSecurityAttributeDefinitionId $customSecurityAttributeDefinitionId -AllowedValueId $allowedValueId

```