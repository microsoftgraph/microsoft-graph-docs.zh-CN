---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ee3ba52d09d6f89b36cec7300aa5c2b62bf14eec8f8379867b1e96f926d31b6f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57219112"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.print().connectors("{id}")
    .buildRequest()
    .delete();

```