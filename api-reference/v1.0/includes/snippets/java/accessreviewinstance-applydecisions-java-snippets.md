---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 823a7d5cf5004b9b944b37815b7683d194d70887437151e76ef110779d1433b7
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105437"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.identityGovernance().accessReviews().definitions("e6cafba0-cbf0-4748-8868-0810c7f4cc06").instances("1234fba0-cbf0-5678-8868-0810c7f49101")
    .applyDecisions()
    .buildRequest()
    .post();

```