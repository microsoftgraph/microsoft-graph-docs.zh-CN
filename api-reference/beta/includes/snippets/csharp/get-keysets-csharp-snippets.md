---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0feee5cf536762760da8491f2de6f32e60790e34fa06861ecc4f5b27bbfa248a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105115"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var keySets = await graphClient.TrustFramework.KeySets
    .Request()
    .GetAsync();

```