---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9a8647d07c23b0b308db3f9b31b9ea4c38e02be8
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62351566"
---
```powershell

Import-Module Microsoft.Graph.People

# A UPN can also be used as -UserId.
Get-MgUserProfileWebsite -UserId $userId

```