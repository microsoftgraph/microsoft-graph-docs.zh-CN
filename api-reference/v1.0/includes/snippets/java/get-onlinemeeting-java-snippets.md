---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c7d856a2a666dbe92d40a8e28945d4619ecf6df5
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50981669"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

OnlineMeetingCollectionPage onlineMeetings = graphClient.communications().onlineMeetings()
    .buildRequest()
    .filter("VideoTeleconferenceId eq '123456789'")
    .get();

```