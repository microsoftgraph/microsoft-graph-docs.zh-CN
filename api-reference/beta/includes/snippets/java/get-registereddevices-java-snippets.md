---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b6569d8e389824f962bcef4bec32ac0bb1097f6e
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48968832"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IDirectoryObjectCollectionWithReferencesPage registeredDevices = graphClient.me().registeredDevices()
    .buildRequest()
    .get();

```