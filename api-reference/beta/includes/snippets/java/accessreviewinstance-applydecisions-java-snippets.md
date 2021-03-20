---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9c4b1ff89db066a207870a00bdfb1438ce800140
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50975050"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.identityGovernance().accessReviews().definitions("04e5c3b2-9db2-40d3-a204-128f4956ae8e").instances("70463350-742e-4909-bfa5-bc23447bd002")
    .applyDecisions()
    .buildRequest()
    .post();

```