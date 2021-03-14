---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c754baa90671b4d1507717e674aed92e0801e886
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50797999"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var schemaExtension = await graphClient.SchemaExtensions["{schemaExtension-id}"]
    .Request()
    .GetAsync();

```