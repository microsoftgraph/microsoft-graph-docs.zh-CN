---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4ef5a193b5b4a1de84669e35f6a0e72edcbe42c1
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50957203"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IPersonNameCollectionPage names = graphClient.me().profile().names()
    .buildRequest()
    .get();

```