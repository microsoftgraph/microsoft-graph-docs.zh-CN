---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4b990df6b735f9ed6068fe947cc8475ff3c8a141
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62131136"
---
```powershell

Import-Module Microsoft.Graph.People

Remove-MgUserProfilePhone -UserId $userId -ItemPhoneId $itemPhoneId

```