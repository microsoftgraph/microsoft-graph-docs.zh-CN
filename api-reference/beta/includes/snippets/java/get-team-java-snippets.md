---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2e794ccce15d5104120f8e1ddc2b7572b7b5d0a9
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50984230"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Team team = graphClient.teams("{id}")
    .buildRequest()
    .get();

```