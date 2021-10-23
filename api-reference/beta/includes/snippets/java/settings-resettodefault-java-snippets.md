---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e81ab19d434af80ac158788690a15c7d43ab11f9b7dc2bb0cc2b6fe78b0f05b7
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57215862"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.compliance().ediscovery().cases("{caseId}").settings()
    .resetToDefault()
    .buildRequest()
    .post();

```