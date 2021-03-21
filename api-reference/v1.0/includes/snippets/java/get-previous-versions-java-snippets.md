---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d4bcc59315eee0f4578963b9d29b40a3d4369ab2
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50984213"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DriveItemVersionCollectionPage versions = graphClient.me().drive().items("{item-id}").versions()
    .buildRequest()
    .get();

```