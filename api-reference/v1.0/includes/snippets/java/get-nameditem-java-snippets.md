---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5e00d671f0b0e0f07979390b8b3a68df95a2c4ec
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50968162"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookNamedItem workbookNamedItem = graphClient.me().drive().items("{id}").workbook().names("{name}")
    .buildRequest()
    .get();

```