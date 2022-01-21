---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fead64aaa669f5b843896259efd197693e7c8236
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62101388"
---
```powershell

Import-Module Microsoft.Graph.PersonalContacts

Remove-MgUserContactFolder -UserId $userId -ContactFolderId $contactFolderId

```