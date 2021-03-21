---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9aecca5fd87537c9bf256f1de5116efcf6f4d9f1
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50984392"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ItemPublicationCollectionPage publications = graphClient.me().profile().publications()
    .buildRequest()
    .get();

```