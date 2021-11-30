---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5b0da6d5b83c7bc08dbb86fa0c9381071b769fc1
ms.sourcegitcommit: e497ed9bb56400bdd2bb53d52ddf057d9966220b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/30/2021
ms.locfileid: "61225507"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var attributeSets = await graphClient.Directory.AttributeSets
    .Request()
    .GetAsync();

```