---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3639353f4787347228cff27073ad5a9e0b812080bace05e268a5c152f9c135ad
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57162497"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var delta = await graphClient.Education.Classes
    .Delta()
    .Request()
    .GetAsync();

```