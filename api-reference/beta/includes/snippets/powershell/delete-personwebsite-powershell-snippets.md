---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 38fc188ce82bc2a7dd2ab73de1a69c278c5b588c
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62120272"
---
```powershell

Import-Module Microsoft.Graph.People

Remove-MgUserProfileWebsite -UserId $userId -PersonWebsiteId $personWebsiteId

```