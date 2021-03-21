---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8211370de40412e6d231a80a2a8695327ee8287f
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50962678"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IWorkbookTableCollectionPage tables = graphClient.me().drive().items("{id}").workbook().worksheets("{id|name}").tables()
    .buildRequest()
    .get();

```