---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 216faf303fea8f26fcf5f36fc8d7910060915f0a
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/25/2021
ms.locfileid: "51210069"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Call call = graphClient.communications().calls("{id}")
    .buildRequest()
    .get();

```