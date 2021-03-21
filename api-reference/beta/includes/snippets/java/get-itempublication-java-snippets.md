---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0edb8bfa95f3b5daced47a62acc15deff611dabf
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50974415"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ItemPublication itemPublication = graphClient.me().profile().publications("{id}")
    .buildRequest()
    .get();

```