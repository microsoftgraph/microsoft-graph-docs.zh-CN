---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f2e9351eb16cfa865d464a77448b56acb48066c5
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62351194"
---
```powershell

Import-Module Microsoft.Graph.People

# A UPN can also be used as -UserId.
Get-MgUserProfile -UserId $userId

```