---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a1e2459c3343eb0d62fa557ec93851437f075aca
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62131122"
---
```powershell

Import-Module Microsoft.Graph.People

Get-MgUserProfileAddress -UserId $userId -ItemAddressId $itemAddressId

```