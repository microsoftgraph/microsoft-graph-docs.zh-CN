---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 137bfd3710864f842bb943be8d86caf8f6d0fd11
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62104756"
---
```powershell

Import-Module Microsoft.Graph.Mail

Get-MgUserMailFolderMessageRule -UserId $userId -MailFolderId $mailFolderId

```