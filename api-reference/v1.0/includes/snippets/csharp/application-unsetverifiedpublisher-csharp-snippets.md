---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9f4b1e267e3655a2ce00c9af4430825858d7b6583d3b163b13a29a5683d0722c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57333559"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Applications["{application-id}"]
    .UnsetVerifiedPublisher()
    .Request()
    .PostAsync();

```