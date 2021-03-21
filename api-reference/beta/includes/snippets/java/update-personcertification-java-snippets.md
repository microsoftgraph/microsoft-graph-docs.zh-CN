---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 754d6bac928b96548e3d0de4a44ecaf88f412818
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50981776"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PersonCertification personCertification = new PersonCertification();
personCertification.issuingAuthority = "International Academy of Marketing Excellence";
personCertification.issuingCompany = "International Academy of Marketing Excellence";

graphClient.users("{userId}").profile().certifications("{id}")
    .buildRequest()
    .patch(personCertification);

```