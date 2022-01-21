---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a586a02722f42e9f54865d5bf39b4a9dd1ab1896
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62129918"
---
```powershell

Import-Module Microsoft.Graph.Teams

Get-MgChatTab -ChatId $chatId -TeamsTabId $teamsTabId -ExpandProperty "teamsApp" 

```