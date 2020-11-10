---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: abd56749850b740abc3ac3a43aaec94ac84abc10
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48964640"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IInformationProtectionLabelCollectionPage labels = graphClient.me().informationProtection().policy().labels()
    .buildRequest()
    .get();

```