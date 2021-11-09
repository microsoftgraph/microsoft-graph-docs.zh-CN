---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d43b0e327f013f62b80e5f468745e4afed32b966
ms.sourcegitcommit: 64d27a0e3dcccc9d857e62aace4153e5d98fb3d0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/03/2021
ms.locfileid: "60736657"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var dataSourceReference = new ReferenceRequestBody
{
    ODataId = "https://graph.microsoft.com/beta/compliance/ediscovery/cases/47746044-fd0b-4a30-acfc-5272b691ba5b/custodians/ab3a628a383045eba344b3caecba3104/userSources/31423539-3846-4333-4136-353644383531"
};

await graphClient.Compliance.Ediscovery.Cases["{ediscovery.case-id}"].SourceCollections["{ediscovery.sourceCollection-id}"].CustodianSources.References
    .Request()
    .AddAsync(dataSourceReference);

```