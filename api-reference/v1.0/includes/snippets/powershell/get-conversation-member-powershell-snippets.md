---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ef9141cf39391972440cdd79c2c089b95831510a
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62129022"
---
```powershell

Import-Module Microsoft.Graph.Teams

Get-MgChatMember -ChatId $chatId -ConversationMemberId $conversationMemberId

```