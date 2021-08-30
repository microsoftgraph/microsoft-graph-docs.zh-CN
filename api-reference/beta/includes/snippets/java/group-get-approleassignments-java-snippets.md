---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bc303e09a9e82e2ba4b643417ce545d502954612511a8957780733eda9ab91a3
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57162213"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AppRoleAssignmentCollectionPage appRoleAssignments = graphClient.groups("7679d9a4-2323-44cd-b5c2-673ec88d8b12").appRoleAssignments()
    .buildRequest()
    .get();

```