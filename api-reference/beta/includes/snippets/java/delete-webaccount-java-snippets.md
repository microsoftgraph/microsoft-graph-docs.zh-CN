---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6a3d25515e3c4b85952a6781d75e7dcc861d382b
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50967828"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.me().profile().webAccounts("{id}")
    .buildRequest()
    .delete();

```