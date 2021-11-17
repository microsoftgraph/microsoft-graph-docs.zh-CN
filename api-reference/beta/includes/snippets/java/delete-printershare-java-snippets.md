---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7ef564b07fff20dfa9c4a8dae90ed1053f2c5f442835ef5d76c7c416022466b9
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105541"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.print().shares("{id}")
    .buildRequest()
    .delete();

```