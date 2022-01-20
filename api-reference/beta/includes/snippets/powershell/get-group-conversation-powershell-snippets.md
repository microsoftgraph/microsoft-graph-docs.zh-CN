---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 35113942867214a493d5143f04e5b8b7b52bccb2
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62127838"
---
```powershell

Import-Module Microsoft.Graph.Groups

Get-MgGroupConversation -GroupId $groupId -ConversationId $conversationId

```