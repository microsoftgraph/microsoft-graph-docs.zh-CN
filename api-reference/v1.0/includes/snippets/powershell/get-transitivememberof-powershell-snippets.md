---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 86df775657061ceb52f13f3dfe5120c1c041e83a
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62110317"
---
```powershell

Import-Module Microsoft.Graph.Users

Get-MgUserTransitiveMemberOf -UserId $userId

```