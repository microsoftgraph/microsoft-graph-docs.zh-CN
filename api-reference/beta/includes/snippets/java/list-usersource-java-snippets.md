---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cbcc1ce066cafd01fd94a7089ea03e438f7e2623
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50971126"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UserSourceCollectionPage userSources = graphClient.compliance().ediscovery().cases("c816dd6f-5af8-40c5-a760-331361e05c60").legalHolds("277107ff-fee3-41a0-a665-a9d7f6c4824f").userSources()
    .buildRequest()
    .get();

```