---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fe76cd27fb140c30178f0b28da2fccf0e8680858
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50970556"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.education().users("{user-id}")
    .buildRequest()
    .delete();

```