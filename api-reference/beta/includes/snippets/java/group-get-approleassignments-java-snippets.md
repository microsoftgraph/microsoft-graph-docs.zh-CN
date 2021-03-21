---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ff4023666c16faf5668430a10898beef79d3c2e1
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50972347"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AppRoleAssignmentCollectionPage appRoleAssignments = graphClient.groups("7679d9a4-2323-44cd-b5c2-673ec88d8b12").appRoleAssignments()
    .buildRequest()
    .get();

```