---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 191d87064e2190b3166b46c0b606efb491e9b688
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62137162"
---
```powershell

Import-Module Microsoft.Graph.Groups

Get-MgGroupEndpoint -GroupId $groupId -EndpointId $endpointId

```