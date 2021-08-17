---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 35f8d25ff533aa1f050449276b79ab32b2963670
ms.sourcegitcommit: 0116750a01323bc9bedd192d4a780edbe7ce0fdc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2021
ms.locfileid: "58258963"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DirectoryObjectCollectionWithReferencesPage appliesTo = graphClient.policies().appManagementPolicies("{id}").appliesTo()
    .buildRequest()
    .get();

```