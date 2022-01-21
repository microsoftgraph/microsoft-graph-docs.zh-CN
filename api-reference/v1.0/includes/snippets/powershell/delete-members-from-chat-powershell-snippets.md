---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 048e39c92ea0a40b30e34ee27bb4c7b3ee484a5b
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62130506"
---
```powershell

Import-Module Microsoft.Graph.Teams

Remove-MgChatMember -ChatId $chatId -ConversationMemberId $conversationMemberId

```