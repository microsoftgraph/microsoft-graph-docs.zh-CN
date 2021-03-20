---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 98880454b7122ee955d925e12a66465951270619
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50971059"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ReviewSet reviewSet = graphClient.compliance().ediscovery().cases("6f65a8e4-c6a0-4cff-8a81-c9ab5df7290d").reviewSets("0157910c-57ce-4e48-bd4b-90f3c88ca32e")
    .buildRequest()
    .get();

```