---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 94f9cabd325abf05150c165b5f67e5aaee86bc6a
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50944141"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IGroupLifecyclePolicyCollectionPage groupLifecyclePolicies = graphClient.groupLifecyclePolicies()
    .buildRequest()
    .get();

```