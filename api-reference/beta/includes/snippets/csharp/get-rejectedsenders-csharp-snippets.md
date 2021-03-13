---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a6c8dfb21dd9b0657fc2046d9db4636819720062
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50789202"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var rejectedSenders = await graphClient.Groups["{group-id}"].RejectedSenders
    .Request()
    .GetAsync();

```