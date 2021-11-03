---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6b5214e7f176960adc04284af158dc37ec6b4b2d
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/03/2021
ms.locfileid: "60687422"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var device = await graphClient.Devices["{device-id}"]
    .Request()
    .Select("id,extensionAttributes")
    .GetAsync();

```