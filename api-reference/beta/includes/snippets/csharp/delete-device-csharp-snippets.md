---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: adceed5218da6f9ed7684a99ab58276858884323c5fe2450415bd746f4bf6c49
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57163708"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Devices["{device-id}"]
    .Request()
    .DeleteAsync();

```