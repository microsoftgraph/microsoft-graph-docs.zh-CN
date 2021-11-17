---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fea61ed825a4d968c0d37539eecec4f74dbb832b605b4bf72017f4216fb75d4c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56902865"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var b2cIdentityUserFlow = await graphClient.Identity.B2cUserFlows["{b2cIdentityUserFlow-id}"]
    .Request()
    .GetAsync();

```