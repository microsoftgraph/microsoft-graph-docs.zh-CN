---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a1a48c085389ad478dca7663619175a9e5fe0977
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50979484"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ItemPhone itemPhone = new ItemPhone();
itemPhone.type = PhoneType.OTHER;

graphClient.users("{userId}").profile().phones("{id}")
    .buildRequest()
    .patch(itemPhone);

```