---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3d2459042021745b42532352eafc39b629ed1cc9
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35885988"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IContactCollectionPage contacts = graphClient.me().contacts()
    .buildRequest()
    .get();

```