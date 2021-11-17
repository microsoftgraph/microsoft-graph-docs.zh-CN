---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9ada861a01c31b50e53c16dd23b01cda7352bae90f46c7e0afceb186fd869457
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57215668"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var extensionProperties = await graphClient.Applications["{application-id}"].ExtensionProperties
    .Request()
    .GetAsync();

```