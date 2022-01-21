---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5574d0646bbe5786bfb7e350b29590c6ad89a116
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62113874"
---
```powershell

Import-Module Microsoft.Graph.Teams

Remove-MgChatInstalledApp -ChatId $chatId -TeamsAppInstallationId $teamsAppInstallationId

```