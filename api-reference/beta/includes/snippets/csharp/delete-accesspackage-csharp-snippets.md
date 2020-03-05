---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cbc72fa0a3e4f766712487da22d72778796796cd
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "37992937"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.IdentityGovernance.EntitlementManagement.AccessPackages["{id}"]
    .Request()
    .DeleteAsync();

```