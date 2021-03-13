---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b7591df3d8e1aee4b0868ed71d310250644743f9
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50798942"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.External.Connections["{externalConnection-id}"].Groups["{externalGroup-id}"]
    .Request()
    .DeleteAsync();

```