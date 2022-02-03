---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4c08f4c819c18971e5b9ce17e16cae45742310e7
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62352700"
---
```powershell

Import-Module Microsoft.Graph.People

# A UPN can also be used as -UserId.
Get-MgUserProfileName -UserId $userId -PersonNameId $personNameId

```