---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: eab26466f14ff5aa5dc49f3a3756224d62bd5240
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50970597"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.me().events("{id}").attachments("{id}")
    .buildRequest()
    .delete();

```