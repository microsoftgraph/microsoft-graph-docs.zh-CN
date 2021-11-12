---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9432bf4630398d36ec430ffc33280f30ce6c1a788f9a9f2e83566d805c4490b2
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57328842"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DirectoryObjectCollectionWithReferencesPage ownedObjects = graphClient.me().ownedObjects()
    .buildRequest()
    .get();

```