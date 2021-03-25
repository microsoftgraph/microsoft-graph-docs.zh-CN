---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 428c7345564ff02ab131b8cb5c68cee8005efff2
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/25/2021
ms.locfileid: "51211209"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedResourceCollectionPage linkedResources = graphClient.me().todo().lists("dfsdc-f9dfdfs-dcsda9").tasks("e2dc-f9cce2-dce29").linkedResources()
    .buildRequest()
    .get();

```