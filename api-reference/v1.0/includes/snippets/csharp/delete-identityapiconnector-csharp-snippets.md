---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b6bfdd9fd6127403bf4ba3350aae680212c38f5218b439a9c203e43a03a04840
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57219347"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Identity.ApiConnectors["{identityApiConnector-id}"]
    .Request()
    .DeleteAsync();

```