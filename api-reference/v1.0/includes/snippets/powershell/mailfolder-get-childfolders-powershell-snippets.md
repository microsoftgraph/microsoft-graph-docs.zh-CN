---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 411c0843e9fa0da1e4f6d0e013bb4b921ab21b68
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62351397"
---
```powershell

Import-Module Microsoft.Graph.Mail

# A UPN can also be used as -UserId.
Get-MgUserMailFolderChildFolder -UserId $userId -MailFolderId $mailFolderId

```