---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 92dd916929bf8a837c995a058410b191e198b46782749ed7a71029283b539f00
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57220378"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DirectoryObjectCollectionWithReferencesPage memberOf = graphClient.servicePrincipals("{id}").memberOf()
    .buildRequest()
    .get();

```