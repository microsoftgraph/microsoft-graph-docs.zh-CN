---
description: 自动生成的文件。请勿修改
ms.openlocfilehash: 7b26c6fb14a0a71409ea9a4903233e62ff027101
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49214333"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var decisions = await graphClient.IdentityGovernance.AccessReviews.Definitions["60860cdd-fb4d-4054-91ba-444404f3baa6"].Instances["14444cdb-6a18-4c08-ba2c-48c02f0a0138"].Decisions
    .Request()
    .Skip(0)
    .Top(100)
    .GetAsync();

```