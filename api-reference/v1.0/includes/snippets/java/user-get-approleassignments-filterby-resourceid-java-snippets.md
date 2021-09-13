---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1c2a5b3d99b3fbd8a95e9763b1608c849b3acf6a0e4a36f05ddcfb946cfc7142
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57106757"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AppRoleAssignmentCollectionPage appRoleAssignments = graphClient.users("cdb555e3-b33e-4fd5-a427-17fadacbdfa7").appRoleAssignments()
    .buildRequest()
    .filter("resourceId eq 8e881353-1735-45af-af21-ee1344582a4d")
    .get();

```