---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 12499e160089b5f1047f9ad8c265623174d6bb039bc75f69ba6e57bc45b85eb4
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57278895"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

SkillProficiency skillProficiency = graphClient.me().profile().skills("{id}")
    .buildRequest()
    .get();

```