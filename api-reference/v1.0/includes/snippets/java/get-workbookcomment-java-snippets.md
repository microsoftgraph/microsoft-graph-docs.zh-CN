---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6027cf2647bea5816ee3ea8d77b40c60adf89439
ms.sourcegitcommit: 2f78ac96a9b0462626a242429055ef824590bd3f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2020
ms.locfileid: "41494848"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookComment workbookComment = graphClient.drive().items("{id}").workbook().comments("{id}")
    .buildRequest()
    .get();

```