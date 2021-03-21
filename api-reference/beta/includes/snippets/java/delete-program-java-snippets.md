---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4bbd600079bc5a2c49bbe15b533b39eedad4e9f1
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50978991"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.programs("7e59d237-2fb0-4e5d-b7bb-d4f9f9129213")
    .buildRequest()
    .delete();

```