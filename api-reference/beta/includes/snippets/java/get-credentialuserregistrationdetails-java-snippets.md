---
description: 自动生成的文件。 不修改
ms.openlocfilehash: c31098720b0e7e4f7bed7c211564ba857eb63ea2
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35871183"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ICredentialUserRegistrationDetailsCollectionPage credentialUserRegistrationDetails = graphClient.reports().credentialUserRegistrationDetails()
    .buildRequest()
    .get();

```