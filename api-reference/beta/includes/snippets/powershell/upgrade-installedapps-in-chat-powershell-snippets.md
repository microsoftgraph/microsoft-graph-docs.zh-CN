---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 00e64b202b93e6dff498ea6cfef9af15c4fd1f77
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2022
ms.locfileid: "66441958"
---
```powershell

Import-Module Microsoft.Graph.Teams

Update-MgChatInstalledApp -ChatId $chatId -TeamsAppInstallationId $teamsAppInstallationId

```