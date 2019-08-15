---
description: 自动生成的文件。 不修改
ms.openlocfilehash: ca7c56969c53a93fee1eb5cb0a71a0650a6e90cd
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/15/2019
ms.locfileid: "36408535"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Agreements["{id}"]
    .Request()
    .DeleteAsync();

```