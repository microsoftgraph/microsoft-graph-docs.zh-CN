---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5a05d718d7da4d5c72caa0aa71c82c17e3e89b36
ms.sourcegitcommit: 2050639c9e9a6b2dab9ce53d6a9fc87e98789b50
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/08/2020
ms.locfileid: "45081166"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var delta = await graphClient.Education.Schools
    .Delta()
    .Request()
    .GetAsync();

```