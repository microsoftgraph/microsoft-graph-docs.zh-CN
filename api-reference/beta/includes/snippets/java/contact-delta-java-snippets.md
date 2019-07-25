---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 2ac50fad13ecb5205eb6edf277e0a618a91a8b5d
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35863492"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IContactDeltaCollectionPage delta = graphClient.me().contactFolders("{id}").contacts()
    .delta()
    .buildRequest()
    .select("displayName")
    .get();

```