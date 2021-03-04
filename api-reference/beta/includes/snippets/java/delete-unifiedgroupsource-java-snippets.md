---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7c6a929052346fb058123a1fd73d2e93e575f9e0
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50445979"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.compliance().ediscovery().cases("{caseId}").custodians("{custodianId}").unifiedGroupSources("{unifiedGroupSourceId}")
    .buildRequest()
    .delete();

```