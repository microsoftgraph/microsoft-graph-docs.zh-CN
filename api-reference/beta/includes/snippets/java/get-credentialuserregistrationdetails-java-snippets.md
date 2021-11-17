---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2a9e15636d23fed9c7217e6ac964a67210cf916fbf5dfac47ef7558f5ba275c2
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57277758"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

CredentialUserRegistrationDetailsCollectionPage credentialUserRegistrationDetails = graphClient.reports().credentialUserRegistrationDetails()
    .buildRequest()
    .get();

```