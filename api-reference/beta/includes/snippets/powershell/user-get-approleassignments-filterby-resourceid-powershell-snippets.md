---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bb84e06e212b0a63b55c0dbae75986013996e028
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62119719"
---
```powershell

Import-Module Microsoft.Graph.Applications

Get-MgUserAppRoleAssignment -UserId $userId -Filter "resourceId eq 8e881353-1735-45af-af21-ee1344582a4d" 

```