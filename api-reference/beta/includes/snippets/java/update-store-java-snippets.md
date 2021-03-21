---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: aadfae679a453176fa15dbbe932e6f9ea5309e3d
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50978872"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Store store = new Store();
store.defaultLanguageTag = "en-US";

graphClient.termStore()
    .buildRequest()
    .patch(store);

```