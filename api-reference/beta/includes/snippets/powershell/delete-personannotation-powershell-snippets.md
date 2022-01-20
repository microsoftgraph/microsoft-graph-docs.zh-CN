---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8e60bbea0b02b9a6901c9b9c2caeeca8201fa45e
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62108453"
---
```powershell

Import-Module Microsoft.Graph.People

Remove-MgUserProfileNote -UserId $userId -PersonAnnotationId $personAnnotationId

```