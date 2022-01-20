---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5b7f034e1d119c08f6cf3f9a1bf61f8d7e38114f
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62109009"
---
```powershell

Import-Module Microsoft.Graph.Education

Get-MgEducationUserAssignment -EducationUserId $educationUserId -ExpandProperty "submissions" 

```