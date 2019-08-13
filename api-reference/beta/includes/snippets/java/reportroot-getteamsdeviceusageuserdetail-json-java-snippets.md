---
description: 自动生成的文件。 不修改
ms.openlocfilehash: e6b6eeee41d5e3844d364ebc259842db4981bf61
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36358939"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ITeamsDeviceUsageUserDetailCollectionPage getTeamsDeviceUsageUserDetail = graphClient.reports()
    .getTeamsDeviceUsageUserDetail("D7")
    .buildRequest()
    .get();

```