---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a93db8993acdca135d5b789f052877c4de532bd8
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62129785"
---
```powershell

Import-Module Microsoft.Graph.People

Get-MgUserProfileEmail -UserId $userId -ItemEmailId $itemEmailId

```