---
description: 自动生成的文件。 不修改
ms.openlocfilehash: aeeafb4a4a63573083ee2e0cdc9e2aa157989966
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35875481"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PrivilegedRoleSettings privilegedRoleSettings = new PrivilegedRoleSettings();
privilegedRoleSettings.id = "9b895d92-2cd3-44c7-9d02-a6ac2d5ea5c3";
privilegedRoleSettings.elevationDuration = "PT8H";
privilegedRoleSettings.notificationToUserOnElevation = false;
privilegedRoleSettings.ticketingInfoOnElevation = true;
privilegedRoleSettings.mfaOnElevation = false;
privilegedRoleSettings.maxElavationDuration = "PT0S";
privilegedRoleSettings.minElevationDuration = "PT0S";
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