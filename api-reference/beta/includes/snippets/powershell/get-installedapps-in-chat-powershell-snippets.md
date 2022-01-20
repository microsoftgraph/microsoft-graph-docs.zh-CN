---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0c181697efc755ef52baa393e9b1b2702094e409
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62094417"
---
```powershell

Import-Module Microsoft.Graph.Teams

Get-MgChatInstalledApp -ChatId $chatId -TeamsAppInstallationId $teamsAppInstallationId

```