---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 00bbf388d11d466249fcb7fa92fb390249881b22
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35887874"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Drive drive = graphClient.groups("{groupId}").drive()
    .buildRequest()
    .get();

```