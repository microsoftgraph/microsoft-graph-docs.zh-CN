---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 52c3418da55ed10a56d0c33ab20a34609e4918cc
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62099680"
---
```powershell

Import-Module Microsoft.Graph.Calendar

Remove-MgGroupEvent -GroupId $groupId -EventId $eventId

```