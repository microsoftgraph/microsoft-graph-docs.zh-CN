---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7df65ce54e72ab1f7ec74a972f0b6ce593c7c106
ms.sourcegitcommit: 36bae3615df41876493b25da478e589d1974f97b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/29/2021
ms.locfileid: "59996648"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var dataSourceReference = new ReferenceRequestBody
{
    OdataId = "https://graph.microsoft.com/beta/compliance/ediscovery/cases/47746044-fd0b-4a30-acfc-5272b691ba5b/custodians/ab3a628a383045eba344b3caecba3104/userSources/31423539-3846-4333-4136-353644383531"
};

await graphClient.Compliance.Ediscovery.Cases["{ediscovery.case-id}"].SourceCollections["{ediscovery.sourceCollection-id}"].CustodianSources.References
    .Request()
    .AddAsync(dataSourceReference);

```