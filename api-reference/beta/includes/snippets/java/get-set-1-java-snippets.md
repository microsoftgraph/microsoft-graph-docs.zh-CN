---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8bf2bb4c840caae5a268cc0171f64db80436838f
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/25/2021
ms.locfileid: "51209945"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

SetCollectionPage sets = graphClient.termStore().groups("{groupId}").sets()
    .buildRequest()
    .get();

```