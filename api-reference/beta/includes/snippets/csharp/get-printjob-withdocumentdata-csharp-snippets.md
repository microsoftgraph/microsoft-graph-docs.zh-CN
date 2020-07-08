---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1b891d9a8ced2ca84feb5a24c955f4eaa43aae75
ms.sourcegitcommit: 2050639c9e9a6b2dab9ce53d6a9fc87e98789b50
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/08/2020
ms.locfileid: "45080619"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var printJob = await graphClient.Print.Printers["86b6d420-7e6b-4797-a05c-af4e56cd81bd"].Jobs["31216"]
    .Request()
    .Expand("documents")
    .GetAsync();

```