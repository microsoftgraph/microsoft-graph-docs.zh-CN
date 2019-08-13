---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 921acda00cebb4548550e758e370f6c043915fb4
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36369416"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Report report = graphClient.reports()
    .getTeamsUserActivityUserDetail("D7")
    .buildRequest()
    .get();

```