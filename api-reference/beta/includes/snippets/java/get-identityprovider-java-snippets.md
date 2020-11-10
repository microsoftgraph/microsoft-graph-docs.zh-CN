---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a29d1e17a2c458ef74bf1ac3bda1ca7e0a01acad
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48953430"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IIdentityProviderCollectionPage identityProviders = graphClient.identityProviders()
    .buildRequest()
    .get();

```