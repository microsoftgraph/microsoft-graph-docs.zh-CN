---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: dba15723bd2de0d3b1414bbe02bfb7c837615dc8
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48609490"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var serviceConfigurationRecords = await graphClient.Domains["contoso.com"].ServiceConfigurationRecords
    .Request()
    .GetAsync();

```