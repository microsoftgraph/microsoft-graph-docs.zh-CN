---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4925ae85511df22f680d73ae7ccfb23b2f3ca647eeac2c88f6bd06aa7ae5cc1c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57409701"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

OpenShiftChangeRequestCollectionPage openShiftChangeRequests = graphClient.teams("{id}").schedule().openShiftChangeRequests()
    .buildRequest()
    .get();

```