---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 11a15d68df94938613d048f62f46ab6d1226a80a4408a4e7dabb26d701e59246
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57163071"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var riskDetection = await graphClient.IdentityProtection.RiskDetections["{riskDetection-id}"]
    .Request()
    .GetAsync();

```