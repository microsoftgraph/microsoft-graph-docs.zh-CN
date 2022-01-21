---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 64a1af784b8133e78510e297e9a3bda79ac0062d
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62106092"
---
```powershell

Import-Module Microsoft.Graph.CloudCommunications

Get-MgUserOnlineMeetingRegistration -UserId $userId -OnlineMeetingId $onlineMeetingId

```