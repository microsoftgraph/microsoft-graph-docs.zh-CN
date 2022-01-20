---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e0f14a5932b1545f9c54636548a03d18d3e1ec8f5fb3db976c6a4d35d438274b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57219845"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

TrustFrameworkKey trustFrameworkKey = graphClient.trustFramework().keySets("{id}")
    .getActiveKey()
    .buildRequest()
    .get();

```