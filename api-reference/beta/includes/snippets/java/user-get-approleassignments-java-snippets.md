---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c15951dca9de1e4ff0c468a7d5454b3463e230cb
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50979890"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AppRoleAssignmentCollectionPage appRoleAssignments = graphClient.users("cdb555e3-b33e-4fd5-a427-17fadacbdfa7").appRoleAssignments()
    .buildRequest()
    .get();

```