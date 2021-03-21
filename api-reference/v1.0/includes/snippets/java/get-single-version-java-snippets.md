---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c27f85be37c3da7dec3fc6db32f5686e871360e1
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50978406"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DriveItemVersion driveItemVersion = graphClient.me().drive().items("{item-id}").versions("{version-id}")
    .buildRequest()
    .get();

```