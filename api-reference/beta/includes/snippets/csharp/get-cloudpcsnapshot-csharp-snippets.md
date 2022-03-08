---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d8785c37b48f9900c185137aaa54ff9d77284245
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63333489"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var cloudPcSnapshot = await graphClient.DeviceManagement.VirtualEndpoint.Snapshots["{cloudPcSnapshot-id}"]
    .Request()
    .GetAsync();

```