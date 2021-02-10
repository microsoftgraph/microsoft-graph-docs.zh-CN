---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c6cd24e5dde8f096e4ffd5481ebff9217dd8c5e6
ms.sourcegitcommit: 48fff935d56fe96e97577a80a3a0aa15c45419ba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/10/2021
ms.locfileid: "50179365"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var custodian = await graphClient.Compliance.Ediscovery.Cases["2192ca408ea2410eba3bec8ae873be6b"].Custodians["45454331323337443946343043464239"]
    .Request()
    .GetAsync();

```