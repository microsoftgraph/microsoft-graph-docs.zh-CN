---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 81a27d238a6438ea5ab7d75fbacbc22c9f08e1fc
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62127392"
---
```powershell

Import-Module Microsoft.Graph.Mail

$params = @{
    DisplayName = "displayName-value"
}

Update-MgUserMailFolder -UserId $userId -MailFolderId $mailFolderId -BodyParameter $params

```