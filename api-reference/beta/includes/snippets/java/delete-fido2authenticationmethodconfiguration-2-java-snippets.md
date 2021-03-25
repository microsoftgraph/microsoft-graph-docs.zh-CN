---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5ef482c8fd2cb05acce1ef6a503d90966b7da231
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/25/2021
ms.locfileid: "51211009"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.policies().authenticationMethodsPolicy().authenticationMethodConfigurations("TemporaryAccessPass")
    .buildRequest()
    .delete();

```