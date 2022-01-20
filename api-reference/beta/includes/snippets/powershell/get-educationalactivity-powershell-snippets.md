---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3e0c892a3c4a3a161c73236ef9cc6461ad06cac2
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62100079"
---
```powershell

Import-Module Microsoft.Graph.People

Get-MgUserProfileEducationalActivity -UserId $userId -EducationalActivityId $educationalActivityId

```