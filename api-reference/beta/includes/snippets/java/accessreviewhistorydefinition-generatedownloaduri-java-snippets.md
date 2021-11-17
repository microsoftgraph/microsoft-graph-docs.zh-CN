---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 010e7a9eddedd4fedcbca62db4591040dc40f06d259e0d985cb54790af075c7f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56902704"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.identityGovernance().accessReviews().historyDefinitions("b2cb022f-b7e1-40f3-9854-c65a40861c38")
    .generateDownloadUri()
    .buildRequest()
    .post();

```