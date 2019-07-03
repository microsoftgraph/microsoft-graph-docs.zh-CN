---
description: 自动生成的文件。 不修改
ms.openlocfilehash: b60eb9de0e26ffa436a8ac1183ce310b65c4dd21
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35509521"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var verificationDnsRecords = await graphClient.Domains["{domain-name}"].VerificationDnsRecords
    .Request()
    .GetAsync();

```