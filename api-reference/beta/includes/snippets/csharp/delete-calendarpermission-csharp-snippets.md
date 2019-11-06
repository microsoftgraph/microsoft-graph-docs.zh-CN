---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e3370f307b43d6b390764c79aa2513285bc382d0
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/05/2019
ms.locfileid: "37994892"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Users["{id}"].Calendar.CalendarPermissions["{id}"]
    .Request()
    .DeleteAsync();

```