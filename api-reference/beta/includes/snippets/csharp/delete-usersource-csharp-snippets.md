---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fdacbfb77c35a3fd88391eba8e750525ea19fa6efcadaefae1a504651094ead0
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57158546"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Compliance.Ediscovery.Cases["{ediscovery.case-id}"].Custodians["{ediscovery.custodian-id}"].UserSources["{ediscovery.userSource-id}"]
    .Request()
    .DeleteAsync();

```