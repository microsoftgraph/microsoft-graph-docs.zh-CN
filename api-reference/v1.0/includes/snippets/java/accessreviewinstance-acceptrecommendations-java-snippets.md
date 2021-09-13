---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b651c14a18787c6512d7d06f4f5559fc781ea437cf16f505a90c1b5f575cf1da
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57162629"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.identityGovernance().accessReviews().definitions("e6cafba0-cbf0-4748-8868-0810c7f4cc06").instances("1234fba0-cbf0-5678-8868-0810c7f91006")
    .acceptRecommendations()
    .buildRequest()
    .post();

```