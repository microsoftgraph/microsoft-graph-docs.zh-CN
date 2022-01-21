---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 53d3763acc3d5981c314affaa5d07bc5aa6ba483
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62094992"
---
```powershell

Import-Module Microsoft.Graph.Calendar

Get-MgUserEventAttachment -UserId $userId -EventId $eventId -AttachmentId $attachmentId

```