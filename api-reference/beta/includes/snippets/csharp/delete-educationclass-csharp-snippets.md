---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9cc5b96a99d86271b47a7cccc8b771d03cf2b1ca
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48620166"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Education.Classes["11022"]
    .Request()
    .DeleteAsync();

```