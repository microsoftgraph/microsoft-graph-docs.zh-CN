---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d100e79f85ea48fe3f135f8996fb182df701a1ad
ms.sourcegitcommit: 5a1373f2ccd9ee813fc60d42e7ac6b115b5f9f66
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/21/2020
ms.locfileid: "44334617"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var rooms = await graphClient.Places["bldg2@contoso.com"].Microsoft.graph.roomlist.Rooms
    .Request()
    .GetAsync();

```