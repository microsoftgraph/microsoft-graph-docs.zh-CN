---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 05835be1ff07378a9b3bf51d9f3ec7b00394e9e1
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50790766"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Contacts["{orgContact-id}"]
    .Request()
    .DeleteAsync();

```