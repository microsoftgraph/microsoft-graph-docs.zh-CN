---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2cd40c5199928378433edcab6b75c9139b9671ad13fdc939032b699cc0a2e7f7
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57273908"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Contract contract = graphClient.contracts("{id}")
    .buildRequest()
    .get();

```