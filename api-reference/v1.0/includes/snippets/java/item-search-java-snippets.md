---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1d2162daa08f13a877304467257d99692bcd007929c14faa3f326ad820cb761f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56903344"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DriveItemSearchCollectionPage search = graphClient.me().drive().root()
    .search(DriveItemSearchParameterSet
        .newBuilder()
        .withQ("Contoso Project")
        .build())
    .buildRequest()
    .get();

```