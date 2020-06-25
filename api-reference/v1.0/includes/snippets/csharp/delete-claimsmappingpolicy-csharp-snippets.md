---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 699c90c6148315b2b0d46b9ebc9fd8a475d05a8b
ms.sourcegitcommit: 1ec5a7be90790aaebdf6d85d93ab0c72b381c9c3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/24/2020
ms.locfileid: "44863830"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Policies.ClaimsMappingPolicies["{id}"]
    .Request()
    .DeleteAsync();

```