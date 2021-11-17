---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d172beeb0d2a83239e5dbb731533d8ed2762a0379b64d9093aa51bf84f352d5d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57328712"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Compliance.Ediscovery.Cases["{ediscovery.case-id}"]
    .Request()
    .DeleteAsync();

```