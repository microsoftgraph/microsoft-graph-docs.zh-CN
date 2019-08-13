---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 5d1323a0852878318b5d717064ce5f8cffb07c36
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36320349"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Report report = graphClient.reports()
    .getYammerActivityUserDetail("D7")
    .buildRequest()
    .get();

```