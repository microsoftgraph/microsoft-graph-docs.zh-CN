---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2e5c30a3af4eca8f104060690e0df743550a3966
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62111478"
---
```powershell

Import-Module Microsoft.Graph.Calendar

Remove-MgUserEventAttachment -UserId $userId -EventId $eventId -AttachmentId $attachmentId

```