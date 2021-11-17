---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fcd184a8b8437a612293b8992c6ec222c8022fea1242caa5d1afa50ae40067f8
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56902598"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ActivityStatisticsCollectionPage activityStatistics = graphClient.me().analytics().activityStatistics()
    .buildRequest()
    .get();

```