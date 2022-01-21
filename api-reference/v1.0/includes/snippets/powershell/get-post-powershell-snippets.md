---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3bd81ee756a7ef353407065bed8061458dd87105
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62117072"
---
```powershell

Import-Module Microsoft.Graph.Groups

Get-MgGroupThreadPost -GroupId $groupId -ConversationThreadId $conversationThreadId -PostId $postId

```