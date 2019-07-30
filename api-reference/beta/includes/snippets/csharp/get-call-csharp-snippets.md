---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 2cdf2041f31f6a5ab20bd74d25579177f5a9807d
ms.sourcegitcommit: 56c0b609dfb1bc5d900956f407d107cdab7086e8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/30/2019
ms.locfileid: "35933830"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var call = await graphClient.App.Calls["{id}"]
    .Request()
    .GetAsync();

```