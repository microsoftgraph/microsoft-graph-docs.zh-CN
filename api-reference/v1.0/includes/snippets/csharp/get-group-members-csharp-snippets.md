---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 87ea6a9955decfca7ce6cadec6c4e5b1c3e6e45d
ms.sourcegitcommit: 7b286637aa332cfd534a41526950b4f6272e0fd7
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/05/2020
ms.locfileid: "41774537"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var members = await graphClient.Groups["{id}"].Members
    .Request()
    .GetAsync();

```