---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7ae1e26d6e28352364212fc1f9385ce4477c9a4d35450807455165585b3f1d8e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56903346"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DriveSearchCollectionPage search = graphClient.me().drive()
    .search(DriveSearchParameterSet
        .newBuilder()
        .withQ("Contoso Project")
        .build())
    .buildRequest()
    .get();

```