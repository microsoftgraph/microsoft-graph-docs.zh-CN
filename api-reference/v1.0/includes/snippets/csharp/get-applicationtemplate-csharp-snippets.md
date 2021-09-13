---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9b224f141b01d5fc9467dbb2cc64b47991517d8d4c917faa01db4e2700c0f940
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57219686"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var applicationTemplate = await graphClient.ApplicationTemplates["{applicationTemplate-id}"]
    .Request()
    .GetAsync();

```