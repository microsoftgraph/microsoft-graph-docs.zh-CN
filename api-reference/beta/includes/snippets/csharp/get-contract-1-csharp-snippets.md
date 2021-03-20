---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d7b14f7e60917d8fe11406770fc09b5b8be51cf6
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50946927"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var contract = await graphClient.Contracts["{contract-id}"]
    .Request()
    .GetAsync();

```