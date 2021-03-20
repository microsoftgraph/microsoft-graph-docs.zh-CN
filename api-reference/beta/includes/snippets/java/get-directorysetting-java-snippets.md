---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ae72a3fa4908b293313d5e69285fb39227572a72
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50970410"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DirectorySetting directorySetting = graphClient.settings("{id}")
    .buildRequest()
    .get();

```