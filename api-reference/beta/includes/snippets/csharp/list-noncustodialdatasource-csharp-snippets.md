---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5b434586f4848eece5ae825a6b2bfcce937415c5
ms.sourcegitcommit: 2a35434fabc76672e21bfc3ed5a1d28f9f3b66bc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2021
ms.locfileid: "52240795"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var noncustodialSources = await graphClient.Compliance.Ediscovery.Cases["{ediscovery.case-id}"].SourceCollections["{ediscovery.sourceCollection-id}"].NoncustodialSources
    .Request()
    .GetAsync();

```