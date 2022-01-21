---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e58aa31c7aa62c0ef00c4a7992dd60c9ddc96f6e
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62094367"
---
```powershell

Import-Module Microsoft.Graph.Applications

Get-MgOnPremisePublishingProfileConnectorMemberOf -OnPremisesPublishingProfileId $onPremisesPublishingProfileId -ConnectorId $connectorId

```