---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 45ec0cb7d3b9271c5bfdce1767136167894bb34a
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/05/2019
ms.locfileid: "37996921"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var languages = await graphClient.Me.Profile.Languages
    .Request()
    .GetAsync();

```