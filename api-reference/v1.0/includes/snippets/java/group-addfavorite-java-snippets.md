---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4322debae5a7402a5b454141767d054844e3415b2f580de96b688ba1c9b98189
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57378774"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.groups("{id}")
    .addFavorite()
    .buildRequest()
    .post();

```