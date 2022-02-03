---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 880406d59b0c77f648acb8a7b17d81505e29fb54
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62341254"
---
```powershell

Import-Module Microsoft.Graph.DeviceManagement.Administration

Get-MgDeviceManagementVirtualEndpointCloudPC -CloudPCId $cloudPCId -Property "id,displayName,imageDisplayName,lastModifiedDateTime,lastRemoteActionResult,lastLoginResult" 

```