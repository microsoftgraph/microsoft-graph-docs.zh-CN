---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 101c4326889d626bcdd7282c01de504d699d5fa4
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62103806"
---
```powershell

Import-Module Microsoft.Graph.Teams

Get-MgChatTab -ChatId $chatId -ExpandProperty "teamsApp" 

```