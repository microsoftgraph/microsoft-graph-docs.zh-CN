---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b2076fce2a3d9a2c06f19bac68cf465561cb36de
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62122287"
---
```powershell

Import-Module Microsoft.Graph.Teams

Get-MgChatMessageHostedContent -ChatId $chatId -ChatMessageId $chatMessageId -ChatMessageHostedContentId $chatMessageHostedContentId

```