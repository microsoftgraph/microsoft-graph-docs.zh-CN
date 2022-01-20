---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c98b601fc4f0918f01a2843396c53791d9a92485
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62120069"
---
```powershell

Import-Module Microsoft.Graph.People

Remove-MgUserProfileProject -UserId $userId -ProjectParticipationId $projectParticipationId

```