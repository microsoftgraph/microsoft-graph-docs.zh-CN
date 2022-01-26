---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bb7293bfeb89dbe4eab14c8f3f7db2d985fa7cb1
ms.sourcegitcommit: 871db8b3f68489d24e2aeafe694725579ee44c47
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/26/2022
ms.locfileid: "62224765"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var userRegistrationDetails = await graphClient.Reports.AuthenticationMethods.UserRegistrationDetails["{userRegistrationDetails-id}"]
    .Request()
    .GetAsync();

```