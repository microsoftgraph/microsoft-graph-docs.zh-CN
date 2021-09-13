---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9ea0499ba5498a2aea9181e9d32367ff3e496ecffaf7af9e80b147cf53cdc5ad
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57163256"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var schemaExtensions = await graphClient.SchemaExtensions
    .Request()
    .Filter("id eq 'graphlearn_test'")
    .GetAsync();

```