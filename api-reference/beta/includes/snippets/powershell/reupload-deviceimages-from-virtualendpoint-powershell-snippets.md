---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1584bf5be4f89d3523d8a9714f46b7c6540da491
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62347752"
---
```powershell

Import-Module Microsoft.Graph.DeviceManagement.Actions

Invoke-MgReuploadDeviceManagementVirtualEndpointDeviceImage -CloudPcDeviceImageId $cloudPcDeviceImageId

```