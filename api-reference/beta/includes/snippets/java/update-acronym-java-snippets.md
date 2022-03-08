---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 16a71587aec1e67d81d584a752a1c18eb3a16c60
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63338335"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Acronym acronym = new Acronym();
acronym.description = "A deep neural network is a neural network with a certain level of complexity, a neural network with more than two layers.";

graphClient.search().acronyms("{acronymsId}")
    .buildRequest()
    .patch(acronym);

```