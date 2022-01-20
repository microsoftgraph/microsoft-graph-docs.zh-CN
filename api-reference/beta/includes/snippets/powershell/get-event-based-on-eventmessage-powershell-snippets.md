---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3e893c263eb629d3e6d1f593af542252d4515678
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62090083"
---
```powershell

Import-Module Microsoft.Graph.Mail

Get-MgUserMessage -UserId $userId -MessageId $messageId -ExpandProperty "microsoft.graph.eventMessage/event" 

```