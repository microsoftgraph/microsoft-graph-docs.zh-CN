---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 710c4c62f38e36a1ca81f494db668a724b256ce1
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62107444"
---
```powershell

Import-Module Microsoft.Graph.Mail

Remove-MgUserMessageExtension -UserId $userId -MessageId $messageId -ExtensionId $extensionId

```