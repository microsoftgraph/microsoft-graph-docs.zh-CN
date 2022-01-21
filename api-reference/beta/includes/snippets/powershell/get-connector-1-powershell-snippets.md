---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: faae785e23355de0dd996374d657bb266e10cd2a
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62090762"
---
```powershell

Import-Module Microsoft.Graph.Applications

Get-MgOnPremisePublishingProfileConnector -OnPremisesPublishingProfileId $onPremisesPublishingProfileId -ConnectorId $connectorId

```