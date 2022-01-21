---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 86c03e18c58d2fb0ff268f026489b305ff85015e
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62128998"
---
```powershell

Import-Module Microsoft.Graph.Teams

Get-MgChatMessage -ChatId $chatId -ChatMessageId $chatMessageId

```