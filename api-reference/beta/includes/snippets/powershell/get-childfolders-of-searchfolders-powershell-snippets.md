---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ed4a718a8f077ba6df28b154c578aadea5eb66ac
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62131097"
---
```powershell

Import-Module Microsoft.Graph.Mail

Get-MgUserMailFolderChildFolder -UserId $userId -MailFolderId $mailFolderId

```