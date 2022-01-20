---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8e652a488cf5701d29a3ec0223cd12f2ddd9b9f9
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62107641"
---
```powershell

Import-Module Microsoft.Graph.Teams

Get-MgChatMessage -ChatId $chatId -Top 2 

```