---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d18614dfed83aa54a1fa068299d45f95777631db
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62088935"
---
```powershell

Import-Module Microsoft.Graph.People

Remove-MgUserProfilePosition -UserId $userId -WorkPositionId $workPositionId

```