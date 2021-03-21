---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: dd231ad69f22602c27c09d0c7871f0578403179a
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50978001"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookOperation workbookOperation = graphClient.me().drive().items("{drive-item-id}").workbook().operations("{operation-id}")
    .buildRequest()
    .get();

```