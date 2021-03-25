---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 508d8833d3498394bdc51b3f5b95e5eb96d80107
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/25/2021
ms.locfileid: "51209223"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Group group = graphClient.termStore().groups("{groupId}")
    .buildRequest()
    .get();

```