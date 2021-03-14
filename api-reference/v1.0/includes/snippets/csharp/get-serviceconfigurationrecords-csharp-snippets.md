---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e8cb4bbef9f3dbf5d5a43a5dcdc40f1c49b71236
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50808868"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var serviceConfigurationRecords = await graphClient.Domains["{domain-id}"].ServiceConfigurationRecords
    .Request()
    .GetAsync();

```