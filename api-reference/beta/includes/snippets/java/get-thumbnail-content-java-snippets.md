---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d9f864939a1fa692b84433388ea907ea23ff12dc
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50983414"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Content content = graphClient.me().drive().items("{item-id}").thumbnails("{thumb-id}").{size}().content()
    .buildRequest()
    .get();

```