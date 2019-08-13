---
description: 自动生成的文件。 不修改
ms.openlocfilehash: daa682aaf0b70683f11ca06d96157e255bccceb5
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36327594"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Report report = graphClient.reports()
    .getOneDriveActivityUserDetail("D7")
    .buildRequest()
    .get();

```