---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1bb2c0ab9f277dd143df99d123e92533edaa07dd5371daa638929957cb6dd40f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57220885"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ItemPatent itemPatent = new ItemPatent();
itemPatent.number = "USPTO-3954432633";
itemPatent.webUrl = "https://patents.gov/3954432633";

graphClient.users("{userId}").profile().patents("{id}")
    .buildRequest()
    .patch(itemPatent);

```