---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f0520be8dcc9a9e6dd27c0297bdfb9c1e9075678
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59021998"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ColumnDefinitionCollectionPage columns = graphClient.sites("{site-id}").columns()
    .buildRequest()
    .get();

```