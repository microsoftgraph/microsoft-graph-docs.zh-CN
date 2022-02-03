---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a23b0106a72a86787eb70b57cd02eb18f26be1fb
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62352295"
---
```powershell

Import-Module Microsoft.Graph.Calendar

# A UPN can also be used as -UserId.
Get-MgUserEventAttachment -UserId $userId -EventId $eventId -AttachmentId $attachmentId

```