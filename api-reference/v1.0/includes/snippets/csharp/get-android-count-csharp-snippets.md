---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: eedb5761ad641ff40d7bf387d6159aac801dfb32a0698baa805f344f66ae0b86
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57333984"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var devices = await graphClient.Devices
    .Request()
    .Header("ConsistencyLevel","eventual")
    .Search("displayName:Android")
    .GetAsync();

```