---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ef28fd77fee5800df3bbd359b4b657c34ba16a3ab9d5c734b0777b8e9c2d5647
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57164042"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var namedLocations = await graphClient.Identity.ConditionalAccess.NamedLocations
    .Request()
    .Filter("createdDateTime ge 2019-09-01T00:00:00Z")
    .GetAsync();

```