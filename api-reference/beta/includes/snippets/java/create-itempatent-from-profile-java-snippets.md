---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2b8683a6375fa1eba867ff86f8441397ef4da045
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50982402"
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