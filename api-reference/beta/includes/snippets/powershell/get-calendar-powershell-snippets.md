---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c7de1c0ff40bbbe4b23169b0e90c6ccd579f901b
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2022
ms.locfileid: "66502842"
---
```powershell

Import-Module Microsoft.Graph.Calendar

# A UPN can also be used as -UserId.
Get-MgUserDefaultCalendar -UserId $userId

```