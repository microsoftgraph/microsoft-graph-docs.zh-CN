---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 57fa180160518e67f7abb92b786b3fcb01c666f8
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62130631"
---
```powershell

Import-Module Microsoft.Graph.PersonalContacts

Get-MgUserContact -UserId $userId -Property "displayName,emailAddresses" 

```