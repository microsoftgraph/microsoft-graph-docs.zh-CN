---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ad735791323eb0c9cbb1f5a3d0927a815eb64b43bdd56a66e3ac121b60e61b3f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57277973"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Set set = new Set();
set.description = "mySet";

graphClient.termStore().sets("{setId}")
    .buildRequest()
    .patch(set);

```