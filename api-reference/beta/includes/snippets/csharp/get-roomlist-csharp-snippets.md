---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7174c4b3edc036e68e6e60c3c22681522edad4db
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50778459"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var place = await graphClient.Places["{place-id}"]
    .Request()
    .GetAsync();

```