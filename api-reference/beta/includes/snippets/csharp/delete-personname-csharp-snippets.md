---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e333397872293910be6390e4417cf79c35be8530
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/05/2019
ms.locfileid: "37997239"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Profile.Names["{id}"]
    .Request()
    .DeleteAsync();

```