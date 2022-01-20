---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1485ff78f7eb58df403b7ecaddef6a65a8744561
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62097055"
---
```powershell

Import-Module Microsoft.Graph.PersonalContacts

Get-MgUserContactFolderChildFolder -UserId $userId -ContactFolderId $contactFolderId

```