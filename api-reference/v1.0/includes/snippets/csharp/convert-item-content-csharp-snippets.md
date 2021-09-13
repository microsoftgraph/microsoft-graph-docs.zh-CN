---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c4b588278ea014f9656cd7fa9f9e92738b85f936ad16f2dfc0f23d02e7c9b2f4
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56902983"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var queryOptions = new List<QueryOption>()
{
    new QueryOption("format", "{format}")
};

var stream = await graphClient.Me.Drive.Items["{driveItem-id}"].Content
    .Request( queryOptions )
    .GetAsync();

```