---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 400472fad624a9e7bd397db346fae72a8e623b41
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62106569"
---
```powershell

Import-Module Microsoft.Graph.PersonalContacts

Remove-MgUserContact -UserId $userId -ContactId $contactId

```