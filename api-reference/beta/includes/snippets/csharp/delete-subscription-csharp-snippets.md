---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 610a689301de81fbd70bb8f95a58295ce1b2d6219938cd09b8005a94d976ce67
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57162729"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Subscriptions["{subscription-id}"]
    .Request()
    .DeleteAsync();

```