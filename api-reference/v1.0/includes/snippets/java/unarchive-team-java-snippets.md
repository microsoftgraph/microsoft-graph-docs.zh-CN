---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 75d9af6bc61634bd0114332b86c6eb4b1a44bbf52277d4655bf966180a5c57e8
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57277374"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.teams("{id}")
    .unarchive()
    .buildRequest()
    .post();

```