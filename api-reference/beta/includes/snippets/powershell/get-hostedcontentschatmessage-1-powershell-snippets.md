---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cb231cc32cdb7ba12fd0b5d160782d11bb8cf0e4
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62123976"
---
```powershell

Import-Module Microsoft.Graph.Teams

Get-MgChatMessageHostedContent -ChatId $chatId -ChatMessageId $chatMessageId

```