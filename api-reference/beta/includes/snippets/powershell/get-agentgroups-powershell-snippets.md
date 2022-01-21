---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b38e07b8120762d0ef5fb0020baa12c9bd3e97b7
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62133292"
---
```powershell

Import-Module Microsoft.Graph.Applications

Get-MgOnPremisePublishingProfileAgentGroup -OnPremisesPublishingProfileId $onPremisesPublishingProfileId -ExpandProperty "agents,publishedResources" 

```