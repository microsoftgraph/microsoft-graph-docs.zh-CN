---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 827735a4787950cede6009d3cb54a00fa8762de4
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62134145"
---
```powershell

Import-Module Microsoft.Graph.Users

Get-MgUserOauth2PermissionGrant -UserId $userId

```