---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ea9bd992cd4b54c1b38b5c9f83bee9d77d6bff49
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35882259"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Channel channel = graphClient.teams("{id}").channels("{id}")
    .buildRequest()
    .get();

```