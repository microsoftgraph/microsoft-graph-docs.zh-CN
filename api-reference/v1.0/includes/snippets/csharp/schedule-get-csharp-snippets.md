---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a7935d4498b034fe9877af372ebde7f020a98b1dc9431e8096c0c1178429b7df
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57279657"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var schedule = await graphClient.Teams["{team-id}"].Schedule
    .Request()
    .GetAsync();

```