---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6d3f8d820313be5b53e5ac539b91e77efcb956cf
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2022
ms.locfileid: "66436812"
---
```powershell

Import-Module Microsoft.Graph.Teams

# A UPN can also be used as -UserId.
Get-MgUserChatMember -UserId $userId -ChatId $chatId

```