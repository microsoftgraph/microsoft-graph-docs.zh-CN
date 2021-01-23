---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 38ba19f64659dd258aac157a35d0b73d1d47f834
ms.sourcegitcommit: 9a5facff47a8d4e05ecd2c6cd68294a948c47c4d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2021
ms.locfileid: "49946313"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var privilegedApproval = await graphClient.PrivilegedApproval["{id}"]
    .Request()
    .GetAsync();

```