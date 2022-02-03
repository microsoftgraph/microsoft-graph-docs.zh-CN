---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e9de42dfdb0a001ab544cd10c88c1208fc30e5bc
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62342336"
---
```powershell

Import-Module Microsoft.Graph.Users.Functions

# A UPN can also be used as -UserId.
Get-MgUserMailFolderMessageDelta -UserId $userId -MailFolderId $mailFolderId

```