---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 90f0fdd28f3b7d5dc9948e0f741ef32f55daab4b
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62132465"
---
```powershell

Import-Module Microsoft.Graph.Mail

Remove-MgUserMessage -UserId $userId -MessageId $messageId

```