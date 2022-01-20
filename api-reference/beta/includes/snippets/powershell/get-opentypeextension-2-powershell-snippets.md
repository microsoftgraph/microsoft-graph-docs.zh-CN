---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5acb505b9d72046139cc200efa10e83dfe8816f4
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62112868"
---
```powershell

Import-Module Microsoft.Graph.Calendar

Get-MgGroupEventExtension -GroupId $groupId -EventId $eventId -ExtensionId $extensionId

```