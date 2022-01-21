---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0a91c81aa7b3ca065112d89d7cdfbd7cc800a030
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62124821"
---
```powershell

Import-Module Microsoft.Graph.PersonalContacts

Get-MgUserContactFolder -UserId $userId -ContactFolderId $contactFolderId

```