---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c18bce0d161d1ee0fc43c9934c335ea4666ebc0ab8d858785f7c199539d1e799
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56902701"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.IdentityGovernance.AccessReviews.HistoryDefinitions["{accessReviewHistoryDefinition-id}"]
    .GenerateDownloadUri()
    .Request()
    .PostAsync();

```