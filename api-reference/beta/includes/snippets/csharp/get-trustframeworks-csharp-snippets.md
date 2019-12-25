---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1d592a63a4876e6220ef8b514cb38874e230708a
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "35716749"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var policies = await graphClient.TrustFramework.Policies
    .Request()
    .GetAsync();

```