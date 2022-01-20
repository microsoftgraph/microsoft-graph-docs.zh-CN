---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2e0500ae7616618a11c1dfce02095df6500dc610
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62122582"
---
```powershell

Import-Module Microsoft.Graph.People

Remove-MgUserProfileAccount -UserId $userId -UserAccountInformationId $userAccountInformationId

```