---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 0f139298e2a18125d244ce889be9e6b863f86f29
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36359343"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ISkypeForBusinessDeviceUsageUserDetailCollectionPage getSkypeForBusinessDeviceUsageUserDetail = graphClient.reports()
    .getSkypeForBusinessDeviceUsageUserDetail("D7")
    .buildRequest()
    .get();

```