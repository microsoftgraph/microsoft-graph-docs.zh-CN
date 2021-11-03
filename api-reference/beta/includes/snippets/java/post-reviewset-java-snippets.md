---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: dc43b1eb2af198bacaf66167b3e76d122df6aebe6df5000372db0987a4f2770c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57106171"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ReviewSet reviewSet = new ReviewSet();
reviewSet.displayName = "My Reviewset 3";

graphClient.compliance().ediscovery().cases("6f65a8e4-c6a0-4cff-8a81-c9ab5df7290d").reviewSets()
    .buildRequest()
    .post(reviewSet);

```