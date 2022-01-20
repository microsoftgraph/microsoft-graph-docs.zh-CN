---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9e84e38216f1bfc5e26439efc357df0efbac3e58
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62117941"
---
```powershell

Import-Module Microsoft.Graph.Teams

$params = @{
    Topic = "Group chat title update"
}

Update-MgChat -ChatId $chatId -BodyParameter $params

```