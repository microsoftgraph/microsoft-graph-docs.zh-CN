---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0b6c4cea4846afcce0e1765dcb60df11cc6c55dd
ms.sourcegitcommit: 9f88b7e41a4a4a4d5f52bd995ce07c6f702bd5d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/01/2020
ms.locfileid: "49521178"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Teams["ece6f0a1-7ca4-498b-be79-edf6c8fc4d82"].Channels["19:56eb04e133944cf69e603c5dac2d292e@thread.skype"].Members["ZWUwZjVhZTItOGJjNi00YWU1LTg0NjYtN2RhZWViYmZhMDYyIyM3Mzc2MWYwNi0yYWM5LTQ2OWMtOWYxMC0yNzlhOGNjMjY3Zjk="]
    .Request()
    .DeleteAsync();

```