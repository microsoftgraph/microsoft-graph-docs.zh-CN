---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6c17b82af9a491f7f193890e82b8d668ba897914
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50980118"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Content response = graphClient.me().drive().items("{item-id}").thumbnails("{thumb-id}").{size}()
    .buildRequest()
    .get();

```