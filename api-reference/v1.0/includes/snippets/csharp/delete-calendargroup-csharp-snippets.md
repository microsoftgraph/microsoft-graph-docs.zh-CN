---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 19ad66ea24b35dc40806ba93039f459a15c2f8e04f50236bf87c750d0710ea98
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57158724"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.CalendarGroups["{calendarGroup-id}"]
    .Request()
    .DeleteAsync();

```