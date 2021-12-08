---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3133935ba0c2da433515d1984af6556a7ade44b7
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/08/2021
ms.locfileid: "61346258"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DirectoryObject directoryObject = new DirectoryObject();
directoryObject.id = "{id}";

graphClient.identityGovernance().entitlementManagement().connectedOrganizations("{id}").externalSponsors().references()
    .buildRequest()
    .post(directoryObject);

```