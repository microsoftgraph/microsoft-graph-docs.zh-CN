---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0345c2675d8f280129e4666fc85d2ef1de06c3192158e26300327a65ce7bb071
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104710"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AppRoleAssignmentCollectionPage appRoleAssignments = graphClient.servicePrincipals("8e881353-1735-45af-af21-ee1344582a4d").appRoleAssignments()
    .buildRequest()
    .get();

```