---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5a6bfcb1b48089f117d9b55462eab1971c8560ae2cc5dec2c2ecf433ce2b52ab
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57161566"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Compliance.Ediscovery.Cases["{ediscovery.case-id}"].NoncustodialDataSources["{ediscovery.noncustodialDataSource-id}"]
    .Release()
    .Request()
    .PostAsync();

```