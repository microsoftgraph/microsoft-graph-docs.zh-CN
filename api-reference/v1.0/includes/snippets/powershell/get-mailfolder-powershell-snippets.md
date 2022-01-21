---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 53225b6a4be0a1e8d0429d352c78b1e37cd130cb
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62130261"
---
```powershell

Import-Module Microsoft.Graph.Mail

Get-MgUserMailFolder -UserId $userId -MailFolderId $mailFolderId

```