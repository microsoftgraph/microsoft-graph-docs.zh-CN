---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 49ea3ef7bc65df714d65db0b8afc5a2b0951311d
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62131521"
---
```powershell

Import-Module Microsoft.Graph.DeviceManagement.Administration

Get-MgDeviceManagementVirtualEndpointAuditEvent -CloudPcAuditEventId $cloudPcAuditEventId

```