---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ed4a15289368d3400ecaeb9e8f0b47cdc48f737d85f2d4c4cf7c676117ed97a4
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57278236"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Identity.ConditionalAccess.Policies["{conditionalAccessPolicy-id}"]
    .Request()
    .DeleteAsync();

```