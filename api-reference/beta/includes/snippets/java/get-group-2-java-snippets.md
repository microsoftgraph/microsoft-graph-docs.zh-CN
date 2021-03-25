---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6dc038a2184f88c891dc64de88b750b3651e99a5
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/25/2021
ms.locfileid: "51208945"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

GroupCollectionPage groups = graphClient.termStore().groups()
    .buildRequest()
    .get();

```