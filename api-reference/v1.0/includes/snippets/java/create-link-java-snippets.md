---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7164e741fe04579be165fc7078b6ca06dfbc38c1
ms.sourcegitcommit: 5575e6607817ba23ceb0b01e2f5fc81e58bdcd1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/22/2020
ms.locfileid: "43771008"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String type = "view";

String scope = "anonymous";

graphClient.me().drive().items("{item-id}")
    .createLink(type,scope,null,null,null)
    .buildRequest()
    .post();

```