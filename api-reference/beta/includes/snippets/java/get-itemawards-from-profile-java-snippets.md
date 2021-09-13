---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 86aa62588a531f3a1f2498a4a2444ba08d95b0e876ca95282d67bb53c666dd83
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105727"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PersonAwardCollectionPage awards = graphClient.me().profile().awards()
    .buildRequest()
    .get();

```