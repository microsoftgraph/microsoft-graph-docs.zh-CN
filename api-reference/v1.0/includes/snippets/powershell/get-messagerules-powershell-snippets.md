---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a34e04e603bc62edc66555a86e9e2ff9adfbe0e3
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62350748"
---
```powershell

Import-Module Microsoft.Graph.Mail

# A UPN can also be used as -UserId.
Get-MgUserMailFolderMessageRule -UserId $userId -MailFolderId $mailFolderId

```