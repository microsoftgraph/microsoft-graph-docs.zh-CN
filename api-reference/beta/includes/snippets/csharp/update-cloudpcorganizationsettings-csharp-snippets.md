---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 92d936bc8893f7f90bee6455f70c1a19b55faf20
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65220285"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var cloudPcOrganizationSettings = new CloudPcOrganizationSettings
{
    UserAccountType = CloudPcUserAccountType.StandardUser,
    OsVersion = CloudPcOperatingSystem.Windows11,
    WindowsSettings = new CloudPcWindowsSettings
    {
        Language = "en-US"
    }
};

await graphClient.DeviceManagement.VirtualEndpoint.OrganizationSettings
    .Request()
    .UpdateAsync(cloudPcOrganizationSettings);

```