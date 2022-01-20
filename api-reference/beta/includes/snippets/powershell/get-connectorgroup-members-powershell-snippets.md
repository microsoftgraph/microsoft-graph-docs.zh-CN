---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c4958cbca9f8d0b0a8a4db214a154c738e0b9f10
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62100408"
---
```powershell

Import-Module Microsoft.Graph.Applications

Get-MgOnPremisePublishingProfileConnectorGroupMember -OnPremisesPublishingProfileId $onPremisesPublishingProfileId -ConnectorGroupId $connectorGroupId

```