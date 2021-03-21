---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 651d6844fe8e7d748b6d24b1c186cfdd949f3929
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50978284"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

OnenoteSectionCollectionPage sections = graphClient.me().onenote().sections()
    .buildRequest()
    .get();

```