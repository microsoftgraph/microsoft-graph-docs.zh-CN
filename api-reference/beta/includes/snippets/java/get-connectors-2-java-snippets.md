---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e860091257f15b9cd839fde2a04fa0913a4005dc
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/25/2021
ms.locfileid: "51210905"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PrintConnectorCollectionPage connectors = graphClient.print().connectors()
    .buildRequest()
    .get();

```