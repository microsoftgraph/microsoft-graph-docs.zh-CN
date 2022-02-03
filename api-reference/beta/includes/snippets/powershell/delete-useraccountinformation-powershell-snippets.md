---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8398cfb5c166a0ed8f1b533dd3d1d154f9bd4d91
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62352636"
---
```powershell

Import-Module Microsoft.Graph.People

# A UPN can also be used as -UserId.
Remove-MgUserProfileAccount -UserId $userId -UserAccountInformationId $userAccountInformationId

```