---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8c19c8898dc3a76980de8e6f89d8e0824c021410
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62099162"
---
```powershell

Import-Module Microsoft.Graph.Users

Remove-MgUserOutlookTaskGroup -UserId $userId -OutlookTaskGroupId $outlookTaskGroupId

```