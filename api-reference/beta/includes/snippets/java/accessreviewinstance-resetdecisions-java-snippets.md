---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b6213a37e26c95eee25baa8049fed45973e62c0fbf0c77434b393b323e400184
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57158596"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.identityGovernance().accessReviews().definitions("0185aab8-9a7e-44b5-ae36-41b923c3bf87").instances("1234aab8-9a7e-44b5-ae36-41b923c3bf87")
    .resetDecisions()
    .buildRequest()
    .post();

```