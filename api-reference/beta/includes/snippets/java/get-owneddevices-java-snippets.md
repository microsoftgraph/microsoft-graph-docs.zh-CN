---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6b1d1061f1813c2add2edaf6250691b40cd69884
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48967328"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IDirectoryObjectCollectionWithReferencesPage ownedDevices = graphClient.me().ownedDevices()
    .buildRequest()
    .get();

```