---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 02de5707189e1d93f142dd829800cac1328637353ca9416c1656d0ee0f881e0d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57274041"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PrintSettings printSettings = graphClient.customRequest("/print/settings", PrintSettings.class)
    .buildRequest()
    .get();

```