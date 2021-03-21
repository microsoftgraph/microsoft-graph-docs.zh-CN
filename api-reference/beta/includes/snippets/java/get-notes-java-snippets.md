---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 13e7be4a917084aa553c615290a8ed9575a0100e
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50968546"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PersonAnnotationCollectionPage notes = graphClient.me().profile().notes()
    .buildRequest()
    .get();

```