---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bc446d05f5e4e272ecf5f37b7a4023ea96f184f9
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/05/2019
ms.locfileid: "37996210"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Profile.WebAccounts["{id}"]
    .Request()
    .DeleteAsync();

```