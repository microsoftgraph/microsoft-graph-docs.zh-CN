---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 859aa938540f022e41b2e69410217122cc0d9929f11af8a6667c7a335e33ccc7
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57106845"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Profile.Positions["{workPosition-id}"]
    .Request()
    .DeleteAsync();

```