---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1fb3687604bf5588ab8d5fb4f3820d1e0fd2871901bcd38abf0e1ef9b9105c09
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57220599"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var securityAction = await graphClient.Security.SecurityActions["{securityAction-id}"]
    .Request()
    .GetAsync();

```