---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 56fbc464e2627bdc8dae5b973795d2b84fda2756401b3ae9b088c14aecbadc21
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57274404"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Domain domain = graphClient.domains("contoso.com")
    .buildRequest()
    .get();

```