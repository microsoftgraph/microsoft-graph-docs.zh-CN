---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a8f24ff5993d8435dc9fac7ec27e865cad24d2f1b7abb533f3ebfc9a80c43ed4
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57220816"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Case _case = new Case();
_case.displayName = "My Case 1";

graphClient.compliance().ediscovery().cases()
    .buildRequest()
    .post(_case);

```