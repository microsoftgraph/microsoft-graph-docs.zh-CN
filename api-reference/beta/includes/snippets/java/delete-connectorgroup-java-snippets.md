---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 691a74bcfc596f30d14223c3c4958957ee4b0a8c3b3c1d8ea169d73a32c36ec6
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105806"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.onPremisesPublishingProfiles("applicationProxy").connectorGroups("{id}")
    .buildRequest()
    .delete();

```