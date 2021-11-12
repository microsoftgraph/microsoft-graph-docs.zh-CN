---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0eef96b7f83984816768f41c8357dcb93fe686fb672ea6ae642baec0a7717207
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57279581"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ItemPhone itemPhone = new ItemPhone();
itemPhone.displayName = "Car Phone";
itemPhone.number = "+7 499 342 22 13";

graphClient.me().profile().phones()
    .buildRequest()
    .post(itemPhone);

```