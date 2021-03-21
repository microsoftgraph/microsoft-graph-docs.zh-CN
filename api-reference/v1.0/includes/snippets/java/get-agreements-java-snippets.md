---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: defef0deea2dc78cecdf31a21a4e66d355a3548f
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50978950"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AgreementCollectionPage agreements = graphClient.identityGovernance().termsOfUse().agreements()
    .buildRequest()
    .get();

```