---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1dbc6a85d57d30767063ecba4551d626ae74469e
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48982116"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IWorkbookCommentCollectionPage comments = graphClient.drive().items("{id}").workbook().comments()
    .buildRequest()
    .get();

```