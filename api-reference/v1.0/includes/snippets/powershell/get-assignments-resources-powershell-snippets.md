---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2921ce29d5c6e12399eac9b7e3f4519d7dfc779f
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62136324"
---
```powershell

Import-Module Microsoft.Graph.Education

Get-MgEducationClassAssignment -EducationClassId $educationClassId -ExpandProperty "resources" 

```