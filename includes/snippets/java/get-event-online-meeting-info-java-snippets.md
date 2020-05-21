---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c7447ed48188da2611b90b660419ec0b7173db87
ms.sourcegitcommit: 5a1373f2ccd9ee813fc60d42e7ac6b115b5f9f66
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/21/2020
ms.locfileid: "44333568"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Event event = graphClient.me().events("AAMkADAGu0AABIGYDZAAA=")
    .buildRequest()
    .select("isOnlineMeeting,onlineMeetingProvider,onlineMeeting")
    .get();

```