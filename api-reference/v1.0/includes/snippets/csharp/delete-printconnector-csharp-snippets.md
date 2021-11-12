---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9a8244b0893be8cb8e3255794a60ef392d8da09a28f30ebaae5d033e2500065f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57218682"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Print.Connectors["{printConnector-id}"]
    .Request()
    .DeleteAsync();

```