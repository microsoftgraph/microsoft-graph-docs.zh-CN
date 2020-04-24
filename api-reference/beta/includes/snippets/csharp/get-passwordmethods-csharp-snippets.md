---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5d2ab1f2db2be560137aaedd704c282814c2b9f4
ms.sourcegitcommit: 5575e6607817ba23ceb0b01e2f5fc81e58bdcd1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/22/2020
ms.locfileid: "43805894"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var passwordMethods = await graphClient.Me.Authentication.PasswordMethods
    .Request()
    .GetAsync();

```