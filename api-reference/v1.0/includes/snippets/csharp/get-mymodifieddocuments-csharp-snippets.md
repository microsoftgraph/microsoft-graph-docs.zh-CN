---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 26a1789f8f32d6f7f8e8487a5a6f0ca17288c4127b3acbcc75d4cf1baf392217
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57163268"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var used = await graphClient.Me.Insights.Used
    .Request()
    .GetAsync();

```