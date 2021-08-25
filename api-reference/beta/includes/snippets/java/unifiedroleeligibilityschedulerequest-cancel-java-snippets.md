---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 15e7cc38a1b0ac27e9adafe77b7518210d4a65cb
ms.sourcegitcommit: 9b8abc940a68dac6ee5da105ca29800cb59775f6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/25/2021
ms.locfileid: "58516060"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.roleManagement().directory().roleEligibilityScheduleRequests("532bef1f-c677-4564-aa6f-811444a4f018")
    .cancel()
    .buildRequest()
    .post();

```