---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3a1738e96eb89120cd33cb01ba928a70a4eeec5a
ms.sourcegitcommit: 5a1373f2ccd9ee813fc60d42e7ac6b115b5f9f66
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/21/2020
ms.locfileid: "44334621"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IRoomListCollectionPage microsoft.graph.roomlist = graphClient.places().microsoft.graph.roomlist()
    .buildRequest()
    .get();

```