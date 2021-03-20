---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f01e7f7d555f032ffcec0fb5a6f33b97a7e65ec2
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50976315"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AudioRoutingGroup audioRoutingGroup = graphClient.communications().calls("{id}").audioRoutingGroups("{id}")
    .buildRequest()
    .get();

```