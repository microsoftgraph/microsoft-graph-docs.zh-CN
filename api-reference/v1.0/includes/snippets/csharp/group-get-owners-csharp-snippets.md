---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b4b23e921f617fbff5c525e5c88c33617ebcb31a7d7ec3587df95d80631171fa
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57107037"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var owners = await graphClient.Groups["{group-id}"].Owners
    .Request()
    .GetAsync();

```