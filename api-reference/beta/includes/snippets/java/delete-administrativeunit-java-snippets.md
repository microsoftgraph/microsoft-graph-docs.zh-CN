---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a5b7146037a9a0e3eb2e4129ca93bf6c79ba4758
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50975365"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.administrativeUnits("{id}")
    .buildRequest()
    .delete();

```