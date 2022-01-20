---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6943095fcac913c5839e1810a74cec26016fb2b6
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62133166"
---
```powershell

Import-Module Microsoft.Graph.People

Remove-MgUserProfileInterest -UserId $userId -PersonInterestId $personInterestId

```