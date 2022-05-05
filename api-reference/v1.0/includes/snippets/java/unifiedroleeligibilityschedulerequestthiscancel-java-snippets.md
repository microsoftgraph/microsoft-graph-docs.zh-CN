---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 15e7cc38a1b0ac27e9adafe77b7518210d4a65cb
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65204814"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.roleManagement().directory().roleEligibilityScheduleRequests("532bef1f-c677-4564-aa6f-811444a4f018")
    .cancel()
    .buildRequest()
    .post();

```