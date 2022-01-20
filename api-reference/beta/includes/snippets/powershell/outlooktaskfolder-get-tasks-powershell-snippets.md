---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1a18988bf7dc18bc6f83623ee4426227b0551cfa
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62089718"
---
```powershell

Import-Module Microsoft.Graph.Users

Get-MgUserOutlookTaskFolderTask -UserId $userId -OutlookTaskFolderId $outlookTaskFolderId

```