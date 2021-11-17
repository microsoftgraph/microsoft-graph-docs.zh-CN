---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 913be121ee0a42f25657ac25260dabcc07a5033fa1e3cd0c59d405d5f85c6658
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57277224"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DirectoryObjectCollectionWithReferencesPage transitiveMemberOf = graphClient.groups("{id}").transitiveMemberOf()
    .buildRequest()
    .get();

```