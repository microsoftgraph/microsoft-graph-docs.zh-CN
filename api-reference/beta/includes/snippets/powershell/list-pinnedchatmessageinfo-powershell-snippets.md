---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ae92160cdebf0e379791de1665aa30354a20a310
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2022
ms.locfileid: "66440719"
---
```powershell

Import-Module Microsoft.Graph.Teams

Get-MgChatPinnedMessage -ChatId $chatId -ExpandProperty "message" 

```