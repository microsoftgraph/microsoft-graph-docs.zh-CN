---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 19641d06221d4c29d76228ebd5bb7e5cc2961f1c
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50800057"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var memberOf = await graphClient.Devices["{device-id}"].MemberOf
    .Request()
    .GetAsync();

```