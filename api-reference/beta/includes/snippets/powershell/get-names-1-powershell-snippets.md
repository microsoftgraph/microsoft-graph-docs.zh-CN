---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e08717d5ff3dd96af9f2397a43afb7e7f682937c
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62350976"
---
```powershell

Import-Module Microsoft.Graph.People

# A UPN can also be used as -UserId.
Get-MgUserProfileName -UserId $userId

```