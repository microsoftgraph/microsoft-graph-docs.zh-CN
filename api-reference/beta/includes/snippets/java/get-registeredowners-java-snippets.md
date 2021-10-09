---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e4995230b4b478d07e2764ad5a468806aa79a8c34eb0b2f716d8ae71f92160a1
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57277349"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DirectoryObjectCollectionWithReferencesPage registeredOwners = graphClient.devices("{id}").registeredOwners()
    .buildRequest()
    .get();

```