---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1ded05c8220970a1f6812cbba8f5368ec11d9ad6
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50968595"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookCommentCollectionPage comments = graphClient.drive().items("{id}").workbook().comments()
    .buildRequest()
    .get();

```