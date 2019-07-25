---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 3f042f38331b912cd961eda5eb66a9918ceffb77
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35892424"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Report report = graphClient.reports()
    .getSkypeForBusinessDeviceUsageUserDetail('D7')
    .buildRequest()
    .get();

```