---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1e751ec1f15e767b4afef054ed7da48d2c4f52452a4c4d04bde3eefebbfcb7ec
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57277562"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Users["{user-id}"].Calendar.CalendarPermissions["{calendarPermission-id}"]
    .Request()
    .DeleteAsync();

```