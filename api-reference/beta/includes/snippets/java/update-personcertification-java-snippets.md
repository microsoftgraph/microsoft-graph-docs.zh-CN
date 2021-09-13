---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3a7e98bc61e844709d25043f11dbc67069cc555c5206edfb448b980be5cb7be6
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57162770"
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