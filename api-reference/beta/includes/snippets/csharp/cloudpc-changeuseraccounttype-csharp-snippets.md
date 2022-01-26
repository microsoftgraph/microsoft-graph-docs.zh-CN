---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 227361017fc9006856295f86e78f075335eae740
ms.sourcegitcommit: 871db8b3f68489d24e2aeafe694725579ee44c47
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/26/2022
ms.locfileid: "62225402"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var userAccountType = CloudPcUserAccountType.Administrator;

await graphClient.DeviceManagement.VirtualEndpoint.CloudPCs["{cloudPC-id}"]
    .ChangeUserAccountType(userAccountType)
    .Request()
    .PostAsync();

```