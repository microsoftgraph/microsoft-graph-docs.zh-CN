---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 238b8855b4e415fcc587d864044da9d18c5bda8e
ms.sourcegitcommit: 82da4012294b046416c9ae93d2294d80dab217f6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/04/2020
ms.locfileid: "48904153"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

TodoTaskList todoTaskList = graphClient.me().todo().lists("AAMkADIyAAAAABrJAAA=")
    .buildRequest()
    .get();

```