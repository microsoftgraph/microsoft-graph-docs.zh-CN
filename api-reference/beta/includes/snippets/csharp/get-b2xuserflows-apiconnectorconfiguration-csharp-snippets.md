---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1b6387a80d18a501983a3b23fc71d5927973a847
ms.sourcegitcommit: a9731e19589dcb5c0c6fe2e24b008c86573ef803
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/13/2021
ms.locfileid: "49843693"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var b2xUserFlows = await graphClient.Identity.B2xUserFlows["B2X_1_testuserflow"]
    .Request()
    .Expand("postAttributeCollection")
    .Select("ApiConnectorConfiguration")
    .GetAsync();

var apiConnectorConfiguration = b2xUserFlows.ApiConnectorConfiguration;

```