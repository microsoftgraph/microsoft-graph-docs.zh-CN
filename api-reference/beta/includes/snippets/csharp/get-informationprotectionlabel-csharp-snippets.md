---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: dd4e634c5322527b125c874625f6dea364b18a17
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/05/2019
ms.locfileid: "37995648"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var informationProtectionLabel = await graphClient.Me.InformationProtection.Policy.Labels["{id}"]
    .Request()
    .GetAsync();

```