---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d778c0f7eb392983baad4acf0f4dd3207c925ae39d47cb99e45c1967eff181c1
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57279479"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.ProgramControls["{programControl-id}"]
    .Request()
    .DeleteAsync();

```