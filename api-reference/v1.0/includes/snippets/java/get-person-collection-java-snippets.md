---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a50111ece3267750b69615f190d1136358aff969
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50975012"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PersonCollectionPage people = graphClient.me().people()
    .buildRequest()
    .get();

```