---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 896c2588afd4adcff0aa50243a8205588bbc0927
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50970555"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

MessageRuleCollectionPage messageRules = graphClient.me().mailFolders("inbox").messageRules()
    .buildRequest()
    .get();

```