---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: dc8fd7abfc536cd23c61e28500cd136a07279b0c
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48974664"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ItemPatent itemPatent = new ItemPatent();
itemPatent.description = "Calculating the intent of a user to purchase an item based on the amount of time they hover their mouse over a given pixel.";
itemPatent.displayName = "Inferring User Intent through browsing behaviors";
itemPatent.isPending = true;
itemPatent.number = "USPTO-3954432633";
itemPatent.webUrl = "https://patents.gov/3954432633";

graphClient.me().profile().patents()
    .buildRequest()
    .post(itemPatent);

```