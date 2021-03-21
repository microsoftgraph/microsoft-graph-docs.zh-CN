---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4146912c0c36ba229f96837a131377eae4c0e56c
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50963881"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IContractCollectionPage contracts = graphClient.contracts()
    .buildRequest()
    .get();

```