---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a47197399e88c98878f49c5588a65bb1dcfdde13
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62095203"
---
```powershell

Import-Module Microsoft.Graph.Mail

Get-MgUserMessage -UserId $userId -MessageId $messageId -Property "internetMessageHeaders" 

```