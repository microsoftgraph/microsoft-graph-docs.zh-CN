---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e78ef690ff4e93542fc8ea5b6bb4e9c97dbcb28d
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62350128"
---
```powershell

Import-Module Microsoft.Graph.Mail

# A UPN can also be used as -UserId.
Get-MgUserMailFolderMessage -UserId $userId -MailFolderId $mailFolderId

```