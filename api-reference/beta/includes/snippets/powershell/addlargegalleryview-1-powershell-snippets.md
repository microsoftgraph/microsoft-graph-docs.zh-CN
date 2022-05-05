---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fe7fc0ab003ea64ffd7122180092ee940c0000bc
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65210444"
---
```powershell

Import-Module Microsoft.Graph.CloudCommunications

$params = @{
    ClientContext = "785f4929-92ca-497b-863f-c778c77c9758"
}

Add-MgCommunicationCallLargeGalleryView -CallId $callId -BodyParameter $params

```