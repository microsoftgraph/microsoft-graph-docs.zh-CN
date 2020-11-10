---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 86264e2ba35f22cfedaa3ba6afd1779eee94e3a5
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48976144"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

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