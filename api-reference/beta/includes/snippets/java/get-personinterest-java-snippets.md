---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9d9b2ccc98139b2630d969a157386212d68e207d
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50970172"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PersonInterest personInterest = graphClient.me().profile().interests("{id}")
    .buildRequest()
    .get();

```