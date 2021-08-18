---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e76553bf5b58b6f63e7997d00b6f9c4f32a4a63f
ms.sourcegitcommit: 0116750a01323bc9bedd192d4a780edbe7ce0fdc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2021
ms.locfileid: "58368868"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DirectoryObjectCollectionWithReferencesPage domainNameReferences = graphClient.domains("contoso.com").domainNameReferences()
    .buildRequest()
    .get();

```