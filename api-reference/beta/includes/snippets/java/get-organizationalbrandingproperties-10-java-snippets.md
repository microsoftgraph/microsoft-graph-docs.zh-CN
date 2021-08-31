---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3b77e0c56321ff8b173f8d768b7a246ab787ab8c487de0420aab1148d01f38aa
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57221515"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String string = graphClient.customRequest("/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/en-US/signInPageText", String.class)
    .buildRequest()
    .get();

```