---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0071b27d64293b3190a9a1e46052f5aed567d28c
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62100450"
---
```powershell

Import-Module Microsoft.Graph.Applications

Get-MgOnPremisePublishingProfileConnectorGroupApplication -OnPremisesPublishingProfileId $onPremisesPublishingProfileId -ConnectorGroupId $connectorGroupId

```