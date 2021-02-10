---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c3e4cb9bc8c34ecf257b35920d6d5b089325e387
ms.sourcegitcommit: 48fff935d56fe96e97577a80a3a0aa15c45419ba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/10/2021
ms.locfileid: "50179483"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var defaultPages = await graphClient.Identity.B2cUserFlows["B2C_1_Customer"].Languages["en"].DefaultPages
    .Request()
    .GetAsync();

```