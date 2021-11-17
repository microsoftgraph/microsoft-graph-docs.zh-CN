---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 54d5268067e02e331d44614489372723dc981f793b5bc326389a32a1c0dee7ad
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57328783"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.identity().userFlows("{id}")
    .buildRequest()
    .delete();

```