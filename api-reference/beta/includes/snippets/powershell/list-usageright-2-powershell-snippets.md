---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 43ed9036a56ed07a936676850f40e7a4b1bd29ce
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62090701"
---
```powershell

Import-Module Microsoft.Graph.Identity.DirectoryManagement

Get-MgDeviceUsageRights -DeviceId $deviceId -Filter "state in ('active', 'suspended') and serviceIdentifier in ('ABCD')" 

```