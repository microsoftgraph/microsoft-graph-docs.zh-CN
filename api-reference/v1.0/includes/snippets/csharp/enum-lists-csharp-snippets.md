---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ccaca0a36c1a6f2d3e4b8227c8fd0438c876a506261922aec24ced5be7ae5173
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57274052"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var lists = await graphClient.Sites["{site-id}"].Lists
    .Request()
    .GetAsync();

```