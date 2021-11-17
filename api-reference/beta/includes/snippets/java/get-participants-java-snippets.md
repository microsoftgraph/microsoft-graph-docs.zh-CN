---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f89cfcc4b4429c0aefaee2a2725fcf045de9073106710d8600cceaedf99b7a80
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57103754"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ParticipantCollectionPage participants = graphClient.communications().calls("7531d31f-d10d-44de-802f-c569dbca451c").participants()
    .buildRequest()
    .get();

```