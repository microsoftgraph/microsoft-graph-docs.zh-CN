---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3b3ca4d578ddd3feb6dcef0e30c5dca05fddb58f
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50981678"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

OrgContactCollectionPage contacts = graphClient.contacts()
    .buildRequest()
    .get();

```