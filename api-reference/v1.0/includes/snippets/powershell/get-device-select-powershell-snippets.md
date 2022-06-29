---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a48b7423802ee79406a10ecbba7545f5a5cec8db
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2022
ms.locfileid: "66444497"
---
```powershell

Import-Module Microsoft.Graph.Identity.DirectoryManagement

Get-MgDevice -DeviceId $deviceId -Property "id,extensionAttributes" 

```