---
description: 自动生成的文件。 不修改
ms.openlocfilehash: d10f78287d70d790c8541156760c04625790a124
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35884135"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IGroupSettingCollectionPage groupSettings = graphClient.groupSettings()
    .buildRequest()
    .get();

```