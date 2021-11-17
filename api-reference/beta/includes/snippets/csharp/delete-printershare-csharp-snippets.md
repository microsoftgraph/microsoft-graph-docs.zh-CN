---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2c06dd9a45f64e637d891576fa4c7585fa102577fc7d97b494eb296ed4cfb4df
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105539"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Print.Shares["{printerShare-id}"]
    .Request()
    .DeleteAsync();

```