---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 483f402e20e9f51a22172fc1292b7a49fd1cab84
ms.sourcegitcommit: 5a1373f2ccd9ee813fc60d42e7ac6b115b5f9f66
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/21/2020
ms.locfileid: "44338912"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String comment = "comment-value";

boolean sendResponse = true;

graphClient.me().events("{id}")
    .tentativelyAccept(null,sendResponse,comment)
    .buildRequest()
    .post();

```