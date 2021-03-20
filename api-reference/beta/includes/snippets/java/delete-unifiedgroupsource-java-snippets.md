---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 450047cd70945e3d804a1bc2a051f4928620dc7d
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50976302"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.compliance().ediscovery().cases("{caseId}").custodians("{custodianId}").unifiedGroupSources("{unifiedGroupSourceId}")
    .buildRequest()
    .delete();

```