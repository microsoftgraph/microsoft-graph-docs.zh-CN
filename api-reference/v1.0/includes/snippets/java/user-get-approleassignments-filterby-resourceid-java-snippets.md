---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2224a2b3328e1f0c1ac1ea9d113d48ada06ba0c0
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50975826"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AppRoleAssignmentCollectionPage appRoleAssignments = graphClient.users("cdb555e3-b33e-4fd5-a427-17fadacbdfa7").appRoleAssignments()
    .buildRequest()
    .filter("resourceId eq 8e881353-1735-45af-af21-ee1344582a4d")
    .get();

```