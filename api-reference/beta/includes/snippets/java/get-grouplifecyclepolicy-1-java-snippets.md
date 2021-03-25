---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0b795814ca759665ab3d0d42bb1f981a871558bb
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/25/2021
ms.locfileid: "51210951"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

GroupLifecyclePolicy groupLifecyclePolicy = graphClient.groupLifecyclePolicies("{id}")
    .buildRequest()
    .get();

```