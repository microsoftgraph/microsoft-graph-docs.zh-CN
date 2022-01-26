---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 289f5e130f0d41f31c25c896aac8741bcfb2b510
ms.sourcegitcommit: 871db8b3f68489d24e2aeafe694725579ee44c47
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/26/2022
ms.locfileid: "62225903"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var operations = await graphClient.Sites["{site-id}"].Operations
    .Request()
    .GetAsync();

```