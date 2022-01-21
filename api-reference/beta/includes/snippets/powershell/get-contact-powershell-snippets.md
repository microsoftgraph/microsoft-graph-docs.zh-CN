---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5dd342d137656279e30abd072e051f9552f8877c
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62100387"
---
```powershell

Import-Module Microsoft.Graph.PersonalContacts

Get-MgUserContact -UserId $userId -ContactId $contactId

```