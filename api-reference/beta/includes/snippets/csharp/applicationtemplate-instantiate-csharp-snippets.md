---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: de73a53f07b34f33e1316001637e146ba4cc3a71
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65220257"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var displayName = "testProperties";

await graphClient.ApplicationTemplates["{applicationTemplate-id}"]
    .Instantiate(displayName)
    .Request()
    .PostAsync();

```