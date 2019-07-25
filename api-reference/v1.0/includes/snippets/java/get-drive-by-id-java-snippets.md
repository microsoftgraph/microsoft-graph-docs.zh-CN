---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 918f4eb49e926d3cdb29e26c0b7cbf5e488b4455
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35887870"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Drive drive = graphClient.drives("{drive-id}")
    .buildRequest()
    .get();

```