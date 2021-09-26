---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 449099e9f622c8603f1745d1454a5075e5cab6de4e6bef0507fcbcd74dfdfea4
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57220232"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var schemaExtension = await graphClient.SchemaExtensions["{schemaExtension-id}"]
    .Request()
    .GetAsync();

```