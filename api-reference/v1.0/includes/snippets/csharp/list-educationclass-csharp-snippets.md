---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8ebc9394a197ce4cc6b75acaaf65d38405dbc996
ms.sourcegitcommit: 503c72036c376a30e08c29df8e7730a7afcab66e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/10/2021
ms.locfileid: "52871346"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var taughtClasses = await graphClient.Education.Users["{educationUser-id}"].TaughtClasses
    .Request()
    .GetAsync();

```