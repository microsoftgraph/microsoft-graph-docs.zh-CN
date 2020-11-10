---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: dc889db96a4051ce9ff76536104184c79c5d69e5
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48957633"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DirectoryObject directoryObject = new DirectoryObject();
directoryObject.id = "{id}";

graphClient.identityGovernance().entitlementManagement().connectedOrganizations("{id}").externalSponsors().references()
    .buildRequest()
    .post(directoryObject);

```