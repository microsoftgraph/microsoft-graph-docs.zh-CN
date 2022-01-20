---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d9b6a50d30c849c64c21d518a220c1f7aa685cd9
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62116310"
---
```powershell

Import-Module Microsoft.Graph.Groups

Get-MgGroupThread -GroupId $groupId -ConversationThreadId $conversationThreadId

```