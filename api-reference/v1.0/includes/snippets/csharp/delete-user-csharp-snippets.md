---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f6c02f3e93d009c76c6ea8db12b53c35e50e14ded3386ef49cc731f6ed6fe60e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57162422"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Users["{user-id}"]
    .Request()
    .DeleteAsync();

```