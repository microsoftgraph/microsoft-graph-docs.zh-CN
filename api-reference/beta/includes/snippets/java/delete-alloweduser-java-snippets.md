---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d5e92b7f51b466011c60850e38c0fc51748fdf20
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50984113"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.print().printerShares("{id}").allowedUsers("{id}").reference()
    .buildRequest()
    .delete();

```