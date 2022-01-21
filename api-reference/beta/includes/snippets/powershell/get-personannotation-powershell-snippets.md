---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4c212d6cbb79768eb8345bbd620682ec7f25bc35
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62118739"
---
```powershell

Import-Module Microsoft.Graph.People

Get-MgUserProfileNote -UserId $userId -PersonAnnotationId $personAnnotationId

```