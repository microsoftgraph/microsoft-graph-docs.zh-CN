---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8a33c63efc97542751d2778bab01144489ea3e3b
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62135958"
---
```powershell

Import-Module Microsoft.Graph.Users

Get-MgUserOutlookMasterCategory -UserId $userId -OutlookCategoryId $outlookCategoryId

```