---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a51258569769757bcc657911b34a8342f92febfb
ms.sourcegitcommit: 9f88b7e41a4a4a4d5f52bd995ce07c6f702bd5d6
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/01/2020
ms.locfileid: "49522531"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var members = await graphClient.Teams["2ab9c796-2902-45f8-b712-7c5a63cf41c4"].Channels["19:20bc1df46b1148e9b22539b83bc66809@thread.skype"].Members
    .Request()
    .GetAsync();

```