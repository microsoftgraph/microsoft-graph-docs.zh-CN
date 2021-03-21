---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 36aad8484e91aed22fc719de400d6a9d8a79bc71
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50970516"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PrintServiceCollectionPage services = graphClient.print().services()
    .buildRequest()
    .get();

```