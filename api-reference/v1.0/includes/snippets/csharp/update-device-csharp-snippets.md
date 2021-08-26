---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6788b22237490d71fcbdddb719b73c6cfe5806972b0b19c8f3873e3cfc2a8ce8
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57278590"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var device = new Device
{
    AccountEnabled = false
};

await graphClient.Devices["{device-id}"]
    .Request()
    .UpdateAsync(device);

```