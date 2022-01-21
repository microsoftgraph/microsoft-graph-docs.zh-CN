---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c67047eb5ebce94fd93b384e9b204e76e412d95b
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62120293"
---
```powershell

Import-Module Microsoft.Graph.People

Get-MgUserProfileCertification -UserId $userId -PersonCertificationId $personCertificationId

```