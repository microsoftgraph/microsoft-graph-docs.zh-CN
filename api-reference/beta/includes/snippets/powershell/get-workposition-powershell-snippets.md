---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 15aed92c96cb2e220d81c7beb3f27e2a33b12a69
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62095530"
---
```powershell

Import-Module Microsoft.Graph.People

Get-MgUserProfilePosition -UserId $userId -WorkPositionId $workPositionId

```