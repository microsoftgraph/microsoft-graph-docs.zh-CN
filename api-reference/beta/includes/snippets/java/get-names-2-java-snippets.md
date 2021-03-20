---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e5f6fe539c0e426a5706353562e5604127174286
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50945754"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IWorkbookNamedItemCollectionPage names = graphClient.me().drive().items("{id}").workbook().names()
    .buildRequest()
    .get();

```