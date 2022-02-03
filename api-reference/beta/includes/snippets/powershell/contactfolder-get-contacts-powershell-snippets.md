---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d8289767b3cd450c860d47146b8d44b7a405a527
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62350926"
---
```powershell

Import-Module Microsoft.Graph.PersonalContacts

# A UPN can also be used as -UserId.
Get-MgUserContactFolderContact -UserId $userId -ContactFolderId $contactFolderId

```