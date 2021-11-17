---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a554a6e7a4f3dc1849fd1f7a4afe1975f3b79be6f162e517b38f7c34a7c880b4
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57278391"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var custodianSources = await graphClient.Compliance.Ediscovery.Cases["{ediscovery.case-id}"].SourceCollections["{ediscovery.sourceCollection-id}"].CustodianSources
    .Request()
    .GetAsync();

```