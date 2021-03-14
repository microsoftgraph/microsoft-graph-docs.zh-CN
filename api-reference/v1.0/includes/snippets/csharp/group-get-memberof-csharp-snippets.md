---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9e1762e0862ac01ba42446584c39d7dff212a7ae
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50788696"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var memberOf = await graphClient.Groups["{group-id}"].MemberOf
    .Request()
    .GetAsync();

```