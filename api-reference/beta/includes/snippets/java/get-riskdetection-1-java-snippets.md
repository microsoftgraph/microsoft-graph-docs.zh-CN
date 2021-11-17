---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7fb4896af921b8f3505c3c0e846390d8b7cc3b7b39a8fbb7594b4af58bf35de1
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57163075"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

RiskDetectionCollectionPage riskDetections = graphClient.riskDetections()
    .buildRequest()
    .get();

```