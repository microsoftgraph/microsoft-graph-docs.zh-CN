---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 615c750d0942241b6a85781cc37e77e1bd35a256
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65211433"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.compliance().ediscovery().cases("{caseId}").sourceCollections("{sourceCollectionId}")
    .purgeData()
    .buildRequest()
    .post();

```