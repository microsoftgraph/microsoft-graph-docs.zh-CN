---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d3440340b6d3fbfa403609c3271bdd96352ea9003bdfb3adfa320bfb1a13c5f3
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57218953"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.communications().calls("57dab8b1-894c-409a-b240-bd8beae78896")
    .buildRequest()
    .delete();

```