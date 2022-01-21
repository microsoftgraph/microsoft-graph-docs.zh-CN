---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ad7cc627471088955f6ca8c638fa6aaa07d882c5
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62116254"
---
```powershell

Import-Module Microsoft.Graph.People

Remove-MgUserProfileAddress -UserId $userId -ItemAddressId $itemAddressId

```