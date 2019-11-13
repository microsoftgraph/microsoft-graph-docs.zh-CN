---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cf9d21794a826b5f0a4afa64a51131f5be466af2
ms.sourcegitcommit: fa08172601324fc01b090f8135fba4600bd1a9f8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/13/2019
ms.locfileid: "38302312"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookApplication workbookApplication = graphClient.me().drive().items("{id}").workbook().application()
    .buildRequest()
    .get();

```