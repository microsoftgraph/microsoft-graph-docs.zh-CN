---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4fc0ec909640dd31ef95f90c63430aae11d8a22b
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62100545"
---
```powershell

Import-Module Microsoft.Graph.Teams

Get-MgChatMessage -ChatId $chatId -Top 2 -Sort "createdDateTime" 

```