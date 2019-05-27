---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 07d042e281b4762a6498ec001dbd9bb9918fc650
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34471576"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var educationSchool = await graphClient.Education.Schools["10001"]
    .Request()
    .GetAsync();

```