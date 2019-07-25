---
description: 自动生成的文件。 不修改
ms.openlocfilehash: a4be7955fa6972189c3125194343b80dce97a51e
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35872742"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ISharePointActivityUserDetailCollectionPage getSharePointActivityUserDetail = graphClient.reports()
    .getSharePointActivityUserDetail('D7')
    .buildRequest()
    .get();

```