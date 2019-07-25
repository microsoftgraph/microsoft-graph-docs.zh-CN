---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3fc2c632fc3568c2c9787088b8c692d1f8710b18
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35884944"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IDirectoryObjectCollectionPage memberOf = graphClient.me().memberOf()
    .buildRequest()
    .get();

```