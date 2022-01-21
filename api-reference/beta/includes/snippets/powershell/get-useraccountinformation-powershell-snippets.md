---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9b57490e91f17c0711385232f38f32f60487461f
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62134965"
---
```powershell

Import-Module Microsoft.Graph.People

Get-MgUserProfileAccount -UserId $userId -UserAccountInformationId $userAccountInformationId

```