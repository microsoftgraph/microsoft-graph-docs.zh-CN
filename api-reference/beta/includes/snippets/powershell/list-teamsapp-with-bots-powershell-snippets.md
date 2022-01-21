---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 53d3ee67a53c87e5959334178d7b4c358a2452b0
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62110077"
---
```powershell

Import-Module Microsoft.Graph.Teams

Get-MgAppCatalogTeamApp -ExpandProperty "appDefinitions(`$expand=bot)" -Filter "appDefinitions/any(a:a/bot ne null)" 

```