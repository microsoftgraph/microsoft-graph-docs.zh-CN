---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9d4c227b7bdea632abdb7a622679ec5abade295e
ms.sourcegitcommit: 0116750a01323bc9bedd192d4a780edbe7ce0fdc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2021
ms.locfileid: "58258966"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DirectoryObjectCollectionWithReferencesPage appliesTo = graphClient.policies().appManagementPolicies("{id}").appliesTo()
    .buildRequest()
    .select("id,appId,displayName,createdDateTime")
    .get();

```