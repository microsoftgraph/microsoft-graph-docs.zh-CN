---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 146143d6b062c3aa899a3613a20d8ccf60ce7edc
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/30/2021
ms.locfileid: "53210693"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var int32 = await graphClient.Contacts["{orgContact-id}"].TransitiveReports.$count
    .Request()
    .GetAsync();

```