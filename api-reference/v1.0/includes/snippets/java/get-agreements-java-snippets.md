---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1be0bde57d6261d55f3221d87d53ca4a36d93560a9936145524a9ddcab7efa17
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56902352"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AgreementCollectionPage agreements = graphClient.identityGovernance().termsOfUse().agreements()
    .buildRequest()
    .get();

```