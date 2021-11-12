---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1dee22f5c83ce4f6d69e3e6a3d592b3f6d0e0faeeb0d94019403c97bdc78ffca
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57162223"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var fido2AuthenticationMethod = await graphClient.Me.Authentication.Fido2Methods["{fido2AuthenticationMethod-id}"]
    .Request()
    .GetAsync();

```