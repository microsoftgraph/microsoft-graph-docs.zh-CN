---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 62f884e3a6993afcf934c428cffb854b2d665d89
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50980888"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ProjectParticipation projectParticipation = graphClient.me().profile().projects("{id}")
    .buildRequest()
    .get();

```