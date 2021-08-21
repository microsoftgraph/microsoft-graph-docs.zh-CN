---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 39920c2e19f4a5dd0b14b281470a989f71501464ceea62873767e0d64eae121c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105125"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PrivilegedApprovalMyRequestsCollectionPage myRequests = graphClient.privilegedApproval()
    .myRequests()
    .buildRequest()
    .get();

```