---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 673f0d08f6e0f8448d0a09f1794ac7a29b680703
ms.sourcegitcommit: 871db8b3f68489d24e2aeafe694725579ee44c47
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/26/2022
ms.locfileid: "62224733"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var userRegistrationDetails = await graphClient.Reports.AuthenticationMethods.UserRegistrationDetails
    .Request()
    .GetAsync();

```