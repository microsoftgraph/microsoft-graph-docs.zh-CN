---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bd47ea67142c1199641aab651865a9366c6820f3e43336e83d6e28b31d1d141a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57163640"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DirectoryObjectCollectionWithReferencesPage ownedObjects = graphClient.servicePrincipals("{id}").ownedObjects()
    .buildRequest()
    .get();

```