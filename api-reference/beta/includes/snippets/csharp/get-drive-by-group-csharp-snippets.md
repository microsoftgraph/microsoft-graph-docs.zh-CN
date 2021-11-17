---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f17b02990b31439e6f0908c0762d38d043d69aeb04ec5892345065625dc3941e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105189"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var drive = await graphClient.Groups["{group-id}"].Drive
    .Request()
    .GetAsync();

```