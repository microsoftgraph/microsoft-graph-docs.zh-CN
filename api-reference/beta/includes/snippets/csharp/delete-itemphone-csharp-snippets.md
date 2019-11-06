---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 739c401daa7a00d8120b2cb84b5aa0723167120b
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/05/2019
ms.locfileid: "37998324"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Profile.Phones["{id}"]
    .Request()
    .DeleteAsync();

```