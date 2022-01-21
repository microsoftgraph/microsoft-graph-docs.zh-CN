---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d1bb160fe637078c60b256911a68710c143e19c3
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62118760"
---
```powershell

Import-Module Microsoft.Graph.People

Get-MgUserProfileAnniversary -UserId $userId -PersonAnnualEventId $personAnnualEventId

```