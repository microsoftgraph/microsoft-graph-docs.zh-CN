---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ca70f7f1b67ac818f2c0b3aab7055fbd65bf9c79
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59022001"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var columns = await graphClient.Sites["{site-id}"].Columns
    .Request()
    .GetAsync();

```