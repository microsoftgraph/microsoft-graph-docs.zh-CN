---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2cb30ed122e18b4de325ae75ce0a2baf2d78a541
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48980718"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IItemPatentCollectionPage patents = graphClient.me().profile().patents()
    .buildRequest()
    .get();

```