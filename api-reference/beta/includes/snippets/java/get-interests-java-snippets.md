---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 562febdec23b094fbcb18d062626c50439e2f950
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50975474"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PersonInterestCollectionPage interests = graphClient.me().profile().interests()
    .buildRequest()
    .get();

```