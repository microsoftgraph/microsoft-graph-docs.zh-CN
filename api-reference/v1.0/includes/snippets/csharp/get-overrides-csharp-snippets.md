---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 782848aec495e19f5e6e0461b5a9d9ac23774cc0ed7943ed430aed24810e39b8
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57279348"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var overrides = await graphClient.Me.InferenceClassification.Overrides
    .Request()
    .GetAsync();

```