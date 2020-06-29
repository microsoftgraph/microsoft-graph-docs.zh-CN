---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d64274d51693ae9cf0e4ad83994f661c83058267
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/26/2020
ms.locfileid: "44900271"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String comment = "comment-value";

boolean sendResponse = true;

graphClient.me().events("{id}")
    .accept(comment,sendResponse)
    .buildRequest()
    .post();

```