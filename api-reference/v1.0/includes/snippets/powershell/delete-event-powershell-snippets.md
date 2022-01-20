---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6ab6303c2a73ce2664da7870697f5560fa88781e
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62104812"
---
```powershell

Import-Module Microsoft.Graph.Calendar

Remove-MgUserEvent -UserId $userId -EventId $eventId

```