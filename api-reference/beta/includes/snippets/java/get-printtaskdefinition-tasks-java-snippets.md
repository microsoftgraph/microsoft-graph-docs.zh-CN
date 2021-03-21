---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7a6b858a8caf94aeb3fcd921977c1871716948d1
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50982866"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PrintTaskCollectionPage tasks = graphClient.print().taskDefinitions("92d72a3d-cad7-4809-8924-43833282b079").tasks()
    .buildRequest()
    .get();

```