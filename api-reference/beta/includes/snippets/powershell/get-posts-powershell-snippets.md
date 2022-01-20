---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 72a9d51d29218edf40ce33d78e9da578c2370e5d
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62106429"
---
```powershell

Import-Module Microsoft.Graph.Groups

Get-MgGroupThreadPost -GroupId $groupId -ConversationThreadId $conversationThreadId

```