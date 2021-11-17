---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 50456ec7655ab85bc4fa0824e05a7dbbf6600709d607e938eedc95b4045a0267
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57220867"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Planner.Buckets["{plannerBucket-id}"]
    .Request()
    .Header("If-Match","W/\"JzEtVGFzayAgQEBAQEBAQEBAQEBAQEBAWCc=\"")
    .DeleteAsync();

```