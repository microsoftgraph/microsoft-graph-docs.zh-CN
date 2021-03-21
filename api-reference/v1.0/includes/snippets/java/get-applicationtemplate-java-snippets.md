---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6eb0ff02e42d63613e2dc2bb2197ba14a6bbc499
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50971695"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ApplicationTemplate applicationTemplate = graphClient.applicationTemplates("{id}")
    .buildRequest()
    .get();

```