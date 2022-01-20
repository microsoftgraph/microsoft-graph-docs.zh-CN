---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 86e416e3ae12ddc15d8e1fc47e4e51dac0893193
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62121062"
---
```powershell

Import-Module Microsoft.Graph.Groups

Remove-MgGroupThread -GroupId $groupId -ConversationThreadId $conversationThreadId

```