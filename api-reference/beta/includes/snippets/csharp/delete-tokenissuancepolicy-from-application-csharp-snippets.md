---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 654becb7b6d7f6627f2dc13516c0a22ebf77b170ccbb2aebe09a91d9adaee7a3
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57215676"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Applications["{application-id}"].TokenIssuancePolicies["{tokenIssuancePolicy-id}"].Reference
    .Request()
    .DeleteAsync();

```