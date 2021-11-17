---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e421689cd88a887ee935c1019acf54bb2dbe1267ce16bb03098570e666c528ab
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57273994"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IdentityUserFlowCollectionPage userFlows = graphClient.identity().userFlows()
    .buildRequest()
    .get();

```