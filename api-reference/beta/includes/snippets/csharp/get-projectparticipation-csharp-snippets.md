---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2478df2e6b0383ae9a345d1d32bcf0c7d07cc6cc
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/05/2019
ms.locfileid: "37996442"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var projectParticipation = await graphClient.Me.Profile.Projects["{id}"]
    .Request()
    .GetAsync();

```