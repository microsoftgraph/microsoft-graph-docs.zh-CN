---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 49a5297f291e1666d144bbd7f6f745d793ddcfd5
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62122773"
---
```powershell

Import-Module Microsoft.Graph.Mail

Get-MgUserMessage -UserId $userId -Property "subject,body,bodyPreview,uniqueBody" 

```