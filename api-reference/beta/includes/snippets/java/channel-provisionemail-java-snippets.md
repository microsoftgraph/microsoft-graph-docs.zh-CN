---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 00ced742c426937ef5bb5cbfae6d9105d1259df0660639ff3563ecf808cdc398
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56903829"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.teams("893075dd-2487-4122-925f-022c42e20265").channels("19:561fbdbbfca848a484f0a6f00ce9dbbd@thread.tacv2")
    .provisionEmail()
    .buildRequest()
    .post();

```