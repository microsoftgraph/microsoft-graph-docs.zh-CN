---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1b5593414f9aff97e7a241e0d08d5454963b27eaf8304bd6e9695daf8e895dc4
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105034"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var userSettings = await graphClient.DeviceManagement.VirtualEndpoint.UserSettings
    .Request()
    .GetAsync();

```