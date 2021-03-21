---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6ad72229ee9e4a731e9abac044c1b061d5cbf878
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50959330"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IWorkbookNamedItemCollectionPage names = graphClient.me().drive().items("{id}").workbook().worksheets("{id|name}").names()
    .buildRequest()
    .get();

```