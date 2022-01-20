---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5197678c3809ee91a86c52376ac9d61e693dab2f
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62134075"
---
```powershell

Import-Module Microsoft.Graph.Groups

Get-MgGroupConversationThread -GroupId $groupId -ConversationId $conversationId

```