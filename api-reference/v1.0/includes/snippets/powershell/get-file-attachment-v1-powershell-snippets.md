---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 690dd30f902b89a7f0b5a5896559591d6e27a2ec
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62136446"
---
```powershell

Import-Module Microsoft.Graph.Mail

Get-MgUserMessageAttachment -UserId $userId -MessageId $messageId -AttachmentId $attachmentId

```