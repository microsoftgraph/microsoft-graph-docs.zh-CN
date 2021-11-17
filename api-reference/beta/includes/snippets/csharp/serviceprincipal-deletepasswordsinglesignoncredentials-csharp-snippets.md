---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bebc0f24ba0c3d1fa8e5aae4abff4a85dbbdefbeb909d8c0380dbee734e49d87
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57164075"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var id = "5793aa3b-cca9-4794-679a240f8b58";

await graphClient.ServicePrincipals["{servicePrincipal-id}"]
    .DeletePasswordSingleSignOnCredentials(id)
    .Request()
    .PostAsync();

```