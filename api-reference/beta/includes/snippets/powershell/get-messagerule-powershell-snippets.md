---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 71b43e6c7ae71c0c7cbec3a6d940ddd94f042cd1
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62113096"
---
```powershell

Import-Module Microsoft.Graph.Mail

Get-MgUserMailFolderMessageRule -UserId $userId -MailFolderId $mailFolderId -MessageRuleId $messageRuleId

```