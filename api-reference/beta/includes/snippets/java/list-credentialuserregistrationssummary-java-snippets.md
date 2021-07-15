---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: da99ec805af3ee6a57959371e9d6ba418fce4260
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/15/2021
ms.locfileid: "53442957"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

CredentialUserRegistrationsSummaryCollectionPage credentialUserRegistrationsSummaries = graphClient.tenantRelationships().managedTenants().credentialUserRegistrationsSummaries()
    .buildRequest()
    .get();

```