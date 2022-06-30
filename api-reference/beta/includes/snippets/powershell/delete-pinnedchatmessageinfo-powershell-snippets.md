---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8a203b35526f9a1adbf4ed48827339216120d52b
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2022
ms.locfileid: "66444702"
---
```powershell

Import-Module Microsoft.Graph.Teams

Remove-MgChatPinnedMessage -ChatId $chatId -PinnedChatMessageInfoId $pinnedChatMessageInfoId

```