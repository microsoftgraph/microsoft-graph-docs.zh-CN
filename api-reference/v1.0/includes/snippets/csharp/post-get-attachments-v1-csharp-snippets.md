---
description: 自动生成的文件。 不修改
ms.openlocfilehash: e9e59f959e20e887d7087b4a36ccf44e999fbd90
ms.sourcegitcommit: 0329bbcd5f1b09a2a6c5f935a30c4560b6eed492
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/27/2019
ms.locfileid: "36636792"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var attachments = await graphClient.Groups["1848753d-185d-4c08-a4e4-6ee40521d115"].Threads["AAQkADJfolA=="].Posts["AAMkADJ-aHAAA="].Attachments
    .Request()
    .GetAsync();

```