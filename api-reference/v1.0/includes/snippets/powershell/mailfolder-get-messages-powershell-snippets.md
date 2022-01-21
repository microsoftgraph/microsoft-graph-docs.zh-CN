---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f64cf63469b1f242ba81dd561e8ab03183df74d8
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62104742"
---
```powershell

Import-Module Microsoft.Graph.Mail

Get-MgUserMailFolderMessage -UserId $userId -MailFolderId $mailFolderId

```