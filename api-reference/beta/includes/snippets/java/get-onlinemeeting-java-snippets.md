---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f3442bf0ac678be268142825b4d83b303819147bbd10c905798bec7df73e21aa
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57101384"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

OnlineMeetingCollectionPage onlineMeetings = graphClient.communications().onlineMeetings()
    .buildRequest()
    .filter("VideoTeleconferenceId eq '123456789'")
    .get();

```