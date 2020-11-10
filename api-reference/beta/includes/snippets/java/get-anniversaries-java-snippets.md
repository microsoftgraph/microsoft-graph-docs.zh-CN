---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a0d3478b6b462b82bea4b14694897383be9fc320
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48970191"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IPersonAnniversaryCollectionPage anniversaries = graphClient.me().profile().anniversaries()
    .buildRequest()
    .get();

```