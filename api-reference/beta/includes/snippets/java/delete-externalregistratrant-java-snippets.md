---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5f517851ec34ba7f31e03153c51b41ada1ab5c61
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62103019"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.me().onlineMeetings("MSpkYzE3Njc0Yy04MWQ5LTRhZGItYmZ").registration().registrants("9d96988d-a66a-46ce-aad7-0b245615b297")
    .buildRequest()
    .delete();

```