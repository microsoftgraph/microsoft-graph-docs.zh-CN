---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b2e5ec80be3c8458b2355badb2c76d4afd0dfd8e
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50971967"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AlertCollectionPage alerts = graphClient.security().alerts()
    .buildRequest()
    .get();

```