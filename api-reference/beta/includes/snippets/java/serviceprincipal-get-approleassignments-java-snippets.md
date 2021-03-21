---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4519b98585ee5c25d98dda3eb63fdc9f85e631de
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50966575"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AppRoleAssignmentCollectionPage appRoleAssignments = graphClient.servicePrincipals("8e881353-1735-45af-af21-ee1344582a4d").appRoleAssignments()
    .buildRequest()
    .get();

```