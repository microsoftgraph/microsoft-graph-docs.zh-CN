---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2c1d14173c62331ca518ec1b77dde01d35c2a860
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62350510"
---
```powershell

Import-Module Microsoft.Graph.Mail

# A UPN can also be used as -UserId.
Get-MgUserMessageAttachment -UserId $userId -MessageId $messageId -AttachmentId $attachmentId

```