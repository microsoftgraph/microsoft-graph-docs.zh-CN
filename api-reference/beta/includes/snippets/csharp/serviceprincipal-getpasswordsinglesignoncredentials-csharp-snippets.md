---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 112d8bdb9574b150a61d1704d68d03379d9327a5
ms.sourcegitcommit: d40d2a9266bd376d713382925323aefab285ed69
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/20/2019
ms.locfileid: "38747836"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var id = "5793aa3b-cca9-4794-679a240f8b58";

await graphClient.ServicePrincipals["{id}"]
    .GetPasswordSingleSignOnCredentials(id)
    .Request()
    .PostAsync();

```