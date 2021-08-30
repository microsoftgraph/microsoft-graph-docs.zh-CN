---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9e05774d15e8abdf4e9464f157d63cab7e849e1cf0f7be8a905883a006681715
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57220808"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ExternalGroup externalGroup = new ExternalGroup();
externalGroup.id = "31bea3d537902000";
externalGroup.displayName = "Contoso Marketing";
externalGroup.description = "The product marketing team";

graphClient.external().connections("contosohr").groups()
    .buildRequest()
    .post(externalGroup);

```