---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 90b3aeac68d29a9f40c5fce24b1f60c2303b7b0b
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62351461"
---
```powershell

Import-Module Microsoft.Graph.People

# A UPN can also be used as -UserId.
Get-MgUserProfileWebAccount -UserId $userId

```