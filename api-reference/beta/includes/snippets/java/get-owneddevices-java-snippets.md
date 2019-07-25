---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 3f0c2be33823bd19d2909000abd2efbbd21e01a8
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35867166"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IDirectoryObjectCollectionPage ownedDevices = graphClient.me().ownedDevices()
    .buildRequest()
    .get();

```