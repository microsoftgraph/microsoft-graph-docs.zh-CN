---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ed2bb061ef847d5cf854faa44ca94a936ae471f1
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/05/2019
ms.locfileid: "37999005"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var application = await graphClient.Applications["{id}"]
    .Request()
    .GetAsync();

```