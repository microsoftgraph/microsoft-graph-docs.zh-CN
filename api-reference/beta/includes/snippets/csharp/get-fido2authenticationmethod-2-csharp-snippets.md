---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 911429bb8f6827d962e608aae63fe488dc3f3a38fa2da27db494181994d85f2c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57273897"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var fido2Methods = await graphClient.Me.Authentication.Fido2Methods
    .Request()
    .GetAsync();

```