---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 055ff18c1cf1c44647c55c91e268d0acf0a178c3
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62118836"
---
```powershell

Import-Module Microsoft.Graph.Calendar

Get-MgGroupEvent -GroupId $groupId -EventId $eventId

```