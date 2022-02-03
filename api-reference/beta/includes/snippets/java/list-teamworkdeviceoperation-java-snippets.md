---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5e6b4ef9437558a3f132693d493ade844cd2c479
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62343398"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

TeamworkDeviceOperationCollectionPage operations = graphClient.teamwork().devices("0f3ce432-e432-0f3c-32e4-3c0f32e43c0f").operations()
    .buildRequest()
    .get();

```