---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0488842d95ec3c06ff89f5844157c94287a78c9e
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/05/2019
ms.locfileid: "37997082"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Profile.Websites["{id}"]
    .Request()
    .DeleteAsync();

```