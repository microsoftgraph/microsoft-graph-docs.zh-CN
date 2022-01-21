---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6bea188a42489e850d38178ee41f28567fc5b411
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62099197"
---
```powershell

Import-Module Microsoft.Graph.Users

Remove-MgUserOutlookTaskFolder -UserId $userId -OutlookTaskFolderId $outlookTaskFolderId

```