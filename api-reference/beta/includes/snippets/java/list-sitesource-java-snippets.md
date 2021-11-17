---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0f75ea06e4546d4d75fea5c40c7d3c3771f128decf123778865819c4f282c041
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57106663"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

SiteSourceCollectionPage siteSources = graphClient.compliance().ediscovery().cases("c816dd6f-5af8-40c5-a760-331361e05c60").legalHolds("277107ff-fee3-41a0-a665-a9d7f6c4824f").siteSources()
    .buildRequest()
    .get();

```