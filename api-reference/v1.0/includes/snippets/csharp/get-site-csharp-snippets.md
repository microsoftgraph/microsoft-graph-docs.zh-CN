---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f5c45ed7d8bf24de4df956067615dcdc19582e47996d3014b2b9c6a408c017e0
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57163466"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var site = await graphClient.Sites["{site-id}"]
    .Request()
    .GetAsync();

```