---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ce31b0f9ed7e343e75841a0014a07238cb41fd6e
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62110075"
---
```powershell

Import-Module Microsoft.Graph.Teams

Get-MgAppCatalogTeamApp -Filter "id eq '876df28f-2e78-423b-94a5-44181bd0e225'" -ExpandProperty "appDefinitions" 

```