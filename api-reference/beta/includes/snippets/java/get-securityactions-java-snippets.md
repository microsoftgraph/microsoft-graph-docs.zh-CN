---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9dce6fb8047c37c2ee4c795088b6bf28e520fc7d
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50967389"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

SecurityActionCollectionPage securityActions = graphClient.security().securityActions()
    .buildRequest()
    .get();

```