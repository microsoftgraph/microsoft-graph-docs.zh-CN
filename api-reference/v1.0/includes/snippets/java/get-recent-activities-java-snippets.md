---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 21abc3cba904d8c1751ebfb411d24ed4b010eb0b
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48983865"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IUserActivityRecentCollectionPage recent = graphClient.me().activities()
    .recent()
    .buildRequest()
    .get();

```