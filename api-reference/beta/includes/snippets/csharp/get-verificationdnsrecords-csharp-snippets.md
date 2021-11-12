---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c2765c06a422263217887c0c818e12576e5e094224fbcc6010acae022b59d115
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104817"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var verificationDnsRecords = await graphClient.Domains["{domain-id}"].VerificationDnsRecords
    .Request()
    .GetAsync();

```