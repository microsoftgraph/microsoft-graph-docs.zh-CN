---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0a389b5d14bdb835eb75dcd6d912b4e257df9aef
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/03/2021
ms.locfileid: "60694832"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var devices = await graphClient.Devices
    .Request()
    .Header("ConsistencyLevel","eventual")
    .Filter("extensionAttributes/extensionAttribute1 eq 'BYOD-Device'")
    .GetAsync();

```