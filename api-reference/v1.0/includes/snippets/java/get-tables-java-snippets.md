---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 8211370de40412e6d231a80a2a8695327ee8287f
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35857267"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IWorkbookTableCollectionPage tables = graphClient.me().drive().items("{id}").workbook().worksheets("{id|name}").tables()
    .buildRequest()
    .get();

```