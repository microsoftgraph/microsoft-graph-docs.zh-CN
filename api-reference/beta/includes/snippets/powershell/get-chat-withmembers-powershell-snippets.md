---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 509c4f0c39544d7ed6fd55c0f46a28529c70d498
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62100642"
---
```powershell

Import-Module Microsoft.Graph.Teams

Get-MgChat -ChatId $chatId -ExpandProperty "members" 

```