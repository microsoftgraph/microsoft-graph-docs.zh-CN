---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 47d0ae7a1f499c0aa9786957be2f79b5c64ab75a
ms.sourcegitcommit: e497ed9bb56400bdd2bb53d52ddf057d9966220b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/30/2021
ms.locfileid: "61223629"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var attributeSet = await graphClient.Directory.AttributeSets["{attributeSet-id}"]
    .Request()
    .GetAsync();

```