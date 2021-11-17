---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4070baecbd856f5e13d50efb17a28d17f9985b9f736efff316583ef13c68e6e9
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57162291"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var bundles = await graphClient.Drive.Bundles
    .Request()
    .GetAsync();

```