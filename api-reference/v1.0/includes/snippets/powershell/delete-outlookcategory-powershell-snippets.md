---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 38dddf0f302e8529b43831f432836d7d2d221222
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62132353"
---
```powershell

Import-Module Microsoft.Graph.Users

Remove-MgUserOutlookMasterCategory -UserId $userId -OutlookCategoryId $outlookCategoryId

```