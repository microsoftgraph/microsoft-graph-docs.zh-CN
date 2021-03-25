---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7d9025acb6c3d55db590d76b8d67a37a79a1794b
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/25/2021
ms.locfileid: "51209338"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

SynchronizationJobCollectionPage jobs = graphClient.servicePrincipals("{id}").synchronization().jobs()
    .buildRequest()
    .get();

```