---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b98469c9aea3b3e007ada2edf617dc1da5f9c10e6cb5403e2cb09df9d04ab095
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57378284"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.education().synchronizationProfiles("{id}")
    .start()
    .buildRequest()
    .post();

```