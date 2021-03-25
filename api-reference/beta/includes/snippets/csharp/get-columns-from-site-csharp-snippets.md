---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ca70f7f1b67ac818f2c0b3aab7055fbd65bf9c79
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/25/2021
ms.locfileid: "51200773"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var columns = await graphClient.Sites["{site-id}"].Columns
    .Request()
    .GetAsync();

```