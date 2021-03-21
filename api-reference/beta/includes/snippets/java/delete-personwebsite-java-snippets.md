---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4f0811839bbc1a71fca21071834bcafd1377ff68
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50982226"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.me().profile().websites("{id}")
    .buildRequest()
    .delete();

```