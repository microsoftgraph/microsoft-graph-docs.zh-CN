---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c933a5f4a5c0c0190db34eb745e5cd4c2f60047b
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62112647"
---
```powershell

Import-Module Microsoft.Graph.Users

Get-MgUserOutlookTaskFolder -UserId $userId -OutlookTaskFolderId $outlookTaskFolderId

```