---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 69e471a915f76a10e0e0beb47f382bc277d544e7
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62110078"
---
```powershell

Import-Module Microsoft.Graph.Teams

Get-MgAppCatalogTeamApp -Filter "distributionMethod eq 'organization'" 

```