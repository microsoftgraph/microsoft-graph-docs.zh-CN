---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1d13fa240fdcd2e2fde4978cd9144d44f93b387a2ea6cf214d5f08615bf0876b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57220611"
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