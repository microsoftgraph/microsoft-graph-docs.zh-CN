---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2940582068ef4bbd4db7aab4e71b06307f8ddb043ac21005c0643ba8d00c28db
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57162964"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.me().onlineMeetings("550fae72-d251-43ec-868c-373732c2704f_19:meeting_M2IzYzczNTItYmY3OC00MDlmLWJjMzUtYmFiMjNlOTY4MGEz@thread.skype")
    .buildRequest()
    .delete();

```