---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d34a1ef0d944740c489a3fba8910ea5b64ba726e
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50981232"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.directoryObjects("{id}")
    .buildRequest()
    .delete();

```