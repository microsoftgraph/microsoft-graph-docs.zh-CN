---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 905eca0525e1007e57696ebadc793c5903ce0b09daa1fc43f4306ba367a44a7b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57106290"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

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