---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5bf2294682f4837ecf82cc9178de057ceb57e1f8
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/03/2021
ms.locfileid: "60694557"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var devices = await graphClient.Devices
    .Request()
    .Select("id,extensionAttributes")
    .GetAsync();

```