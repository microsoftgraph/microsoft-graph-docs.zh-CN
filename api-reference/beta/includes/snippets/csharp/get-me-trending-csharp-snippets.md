---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0df7c48909799c988e8daf4e0cd89852c2b3783a
ms.sourcegitcommit: 9faca60f0cc4ee9d6dce33fd25c72e14b5487d34
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/29/2020
ms.locfileid: "46509673"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var trending = await graphClient.Me.Insights.Trending
    .Request()
    .GetAsync();

```