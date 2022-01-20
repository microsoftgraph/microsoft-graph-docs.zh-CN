---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 38ed3babeda68cf39372d5d0b6bd4f690aaf581b
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62108830"
---
```powershell

Import-Module Microsoft.Graph.Groups

Remove-MgGroupConversation -GroupId $groupId -ConversationId $conversationId

```