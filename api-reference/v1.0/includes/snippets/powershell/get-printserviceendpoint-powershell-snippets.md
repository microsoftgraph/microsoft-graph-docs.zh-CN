---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: beeee9e2cc89f56ae7c12cd32433577b2864988f
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62116954"
---
```powershell

Import-Module Microsoft.Graph.Devices.CloudPrint

Get-MgPrintServiceEndpoint -PrintServiceId $printServiceId -PrintServiceEndpointId $printServiceEndpointId

```