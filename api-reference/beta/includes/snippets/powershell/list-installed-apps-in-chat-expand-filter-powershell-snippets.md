---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2b2858a40f2be2d410a55d4cc7702f734efdca32
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62128036"
---
```powershell

Import-Module Microsoft.Graph.Teams

Get-MgChatInstalledApp -ChatId $chatId -ExpandProperty "teamsApp,teamsAppDefinition" -Filter "teamsApp/externalId eq 'cf1ba4c7-f94e-4d80-ba90-5594b641a8ee'" 

```