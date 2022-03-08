---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 927f27cb221ffb0ded442bfb9ba84a80dbd1a64b
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63338327"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Acronym acronym = new Acronym();
acronym.displayName = "DNN";
acronym.standsFor = "Deep Neural Network";
acronym.description = "A deep neural network is a neural network with a certain level of complexity, a neural network with more than two layers.";
acronym.webUrl = "http://microsoft.com/deep-neural-network";
acronym.state = AnswerState.DRAFT;

graphClient.search().acronyms()
    .buildRequest()
    .post(acronym);

```