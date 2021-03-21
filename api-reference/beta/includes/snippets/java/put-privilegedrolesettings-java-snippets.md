---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: efdce06dfe5df65ec47d63d43bd9aa99530dd2a2
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50971230"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PrivilegedRoleSettings privilegedRoleSettings = new PrivilegedRoleSettings();
privilegedRoleSettings.id = "9b895d92-2cd3-44c7-9d02-a6ac2d5ea5c3";
privilegedRoleSettings.elevationDuration = DatatypeFactory.newInstance().newDuration("PT8H");
privilegedRoleSettings.notificationToUserOnElevation = false;
privilegedRoleSettings.ticketingInfoOnElevation = true;
privilegedRoleSettings.mfaOnElevation = false;
privilegedRoleSettings.maxElavationDuration = DatatypeFactory.newInstance().newDuration("PT0S");
privilegedRoleSettings.minElevationDuration = DatatypeFactory.newInstance().newDuration("PT0S");
privilegedRoleSettings.lastGlobalAdmin = false;
privilegedRoleSettings.isMfaOnElevationConfigurable = true;
privilegedRoleSettings.approvalOnElevation = false;
LinkedList<String> approverIdsList = new LinkedList<String>();
approverIdsList.add("e2b2a2fb-13d7-495c-adc9-941fe966793f");
approverIdsList.add("22770e3f-b9b4-418e-9dea-d0e3d2f275dd");
privilegedRoleSettings.approverIds = approverIdsList;

graphClient.privilegedRoles("{id}").settings()
    .buildRequest()
    .put(privilegedRoleSettings);

```