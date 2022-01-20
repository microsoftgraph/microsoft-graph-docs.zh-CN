---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3f291372dbf83a38058b25c47af3f402afdb09dc
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62122772"
---
```powershell

Import-Module Microsoft.Graph.Mail

Get-MgUserMessage -UserId $userId -Property "sender,subject" 

```