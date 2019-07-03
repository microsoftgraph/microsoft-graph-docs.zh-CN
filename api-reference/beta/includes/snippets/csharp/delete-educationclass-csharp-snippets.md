---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 9cc5b96a99d86271b47a7cccc8b771d03cf2b1ca
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35463539"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Education.Classes["11022"]
    .Request()
    .DeleteAsync();

```