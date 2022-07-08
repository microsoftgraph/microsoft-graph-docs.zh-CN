---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a4330c0c2bd10f80afd25c8f685cb0394ed86c86
ms.sourcegitcommit: 54ba08a80db85b9e84813387e8c4416eca44fa8e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/26/2022
ms.locfileid: "65695227"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DeviceRegistrationPolicy deviceRegistrationPolicy = new DeviceRegistrationPolicy();
deviceRegistrationPolicy.id = "deviceRegistrationPolicy";
deviceRegistrationPolicy.displayName = "Device Registration Policy";
deviceRegistrationPolicy.description = "Tenant-wide policy that manages intial provisioning controls using quota restrictions, additional authentication and authorization checks";
deviceRegistrationPolicy.userDeviceQuota = 50;
deviceRegistrationPolicy.multiFactorAuthConfiguration = MultiFactorAuthConfiguration.NOT_REQUIRED;
AzureADRegistrationPolicy azureADRegistration = new AzureADRegistrationPolicy();
azureADRegistration.appliesTo = PolicyScope.NONE;
azureADRegistration.isAdminConfigurable = false;
LinkedList<String> allowedUsersList = new LinkedList<String>();
azureADRegistration.allowedUsers = allowedUsersList;
LinkedList<String> allowedGroupsList = new LinkedList<String>();
azureADRegistration.allowedGroups = allowedGroupsList;
deviceRegistrationPolicy.azureADRegistration = azureADRegistration;
AzureAdJoinPolicy azureADJoin = new AzureAdJoinPolicy();
azureADJoin.appliesTo = PolicyScope.NONE;
azureADJoin.isAdminConfigurable = true;
LinkedList<String> allowedUsersList1 = new LinkedList<String>();
azureADJoin.allowedUsers = allowedUsersList1;
LinkedList<String> allowedGroupsList1 = new LinkedList<String>();
azureADJoin.allowedGroups = allowedGroupsList1;
deviceRegistrationPolicy.azureADJoin = azureADJoin;

graphClient.deviceRegistrationPolicy()
    .buildRequest()
    .put(deviceRegistrationPolicy);

```