---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 54c8a922c15fce955f451f98c49a026ca78649e135d475770d414870793e94ab
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57274249"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var int32 = await graphClient.Groups["{group-id}"].TransitiveMembers.$count
    .Request()
    .Header("ConsistencyLevel","eventual")
    .GetAsync();

```