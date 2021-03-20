---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6bd47966a42684136e58e25d76173e42b5885b82
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50971574"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

TrustFrameworkKey trustFrameworkKey = graphClient.trustFramework().keySets("{id}")
    .getActiveKey()
    .buildRequest()
    .get();

```