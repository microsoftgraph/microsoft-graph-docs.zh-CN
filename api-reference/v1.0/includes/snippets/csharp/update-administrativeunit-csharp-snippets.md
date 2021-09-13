---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b004e11576896e81e575a835dc4559d40cc9c9274ec3066907a21c78e73d3ee2
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57277264"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var administrativeUnit = new AdministrativeUnit
{
    DisplayName = "displayName-value",
    Description = "description-value",
    Visibility = "visibility-value"
};

await graphClient.Directory.AdministrativeUnits["{administrativeUnit-id}"]
    .Request()
    .UpdateAsync(administrativeUnit);

```