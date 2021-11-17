---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f3051223dd4100b583ffc26c6af227e393ca80e5bb4284d6d52ed945c990ad7f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104039"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var delta = await graphClient.Applications
    .Delta()
    .Request()
    .GetAsync();

```