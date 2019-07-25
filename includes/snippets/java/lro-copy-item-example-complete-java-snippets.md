---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 9c90eaa0fdbc3fd8740aced61d4eed328f1152eb
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35880994"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DriveItem driveItem = graphClient.me().drive().items("{item-id}")
    .buildRequest()
    .get();

```