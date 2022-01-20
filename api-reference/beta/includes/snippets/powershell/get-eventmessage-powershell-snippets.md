---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6cf90acdd1d8a3e471c9609a256ea449a8eb2cdb
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62090084"
---
```powershell

Import-Module Microsoft.Graph.Mail

Get-MgUserMessage -UserId $userId -MessageId $messageId

```