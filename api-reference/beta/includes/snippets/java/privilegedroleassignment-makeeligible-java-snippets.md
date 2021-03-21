---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 748f548142b94335715c88629e356d9debc6a77b
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50983771"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.privilegedRoleAssignments("{id}")
    .makeEligible()
    .buildRequest()
    .post();

```