---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 195c4597803e12efb48f0c05fcaa427fa060b016fa4b2353be8b4c22b86b8c4a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57378580"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Security.TiIndicators["{tiIndicator-id}"]
    .Request()
    .DeleteAsync();

```