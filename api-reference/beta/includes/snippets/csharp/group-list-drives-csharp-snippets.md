---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6dd2c6a8f068c1d02696e3835f32d844b640d1d18e2e37cd4a3c353e6e3222a5
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57161729"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var drives = await graphClient.Groups["{group-id}"].Drives
    .Request()
    .GetAsync();

```