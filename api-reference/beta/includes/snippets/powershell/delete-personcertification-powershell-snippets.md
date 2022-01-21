---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ba259334081046b4fee2cb5f49512c62578f3a2c
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62123163"
---
```powershell

Import-Module Microsoft.Graph.People

Remove-MgUserProfileCertification -UserId $userId -PersonCertificationId $personCertificationId

```