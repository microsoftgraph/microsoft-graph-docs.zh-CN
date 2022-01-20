---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6491fa3181fcacc61fab274e2866be6f9aea0503
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62120307"
---
```powershell

Import-Module Microsoft.Graph.People

Get-MgUserProfileName -UserId $userId -PersonNameId $personNameId

```