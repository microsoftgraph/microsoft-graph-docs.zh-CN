---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 267e76f5edddb5c38514d979a1ede154b13a35f4
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62352742"
---
```powershell

Import-Module Microsoft.Graph.Calendar

# A UPN can also be used as -UserId.
Get-MgUserCalendarGroup -UserId $userId

```