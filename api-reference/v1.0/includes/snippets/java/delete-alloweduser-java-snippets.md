---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 73ad6a16d3d0070e21386d33329ad46c0fe93c12550cd38df26bcd1b85181dcc
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57279723"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.print().shares("{printerShareId}").allowedUsers("{userId}").reference()
    .buildRequest()
    .delete();

```