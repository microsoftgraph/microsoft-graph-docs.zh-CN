---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2ba2e41555b60d01438b4b61f53f0d3ddc0b6729
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62134597"
---
```powershell

Import-Module Microsoft.Graph.Groups

Get-MgGroupThreadPostExtension -GroupId $groupId -ConversationThreadId $conversationThreadId -PostId $postId -ExtensionId $extensionId

```