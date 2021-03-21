---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6c1fa84a5dbf219405044e9d1a01c01152a0058d
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50969342"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EventCollectionPage events = graphClient.groups("{id}").events()
    .buildRequest()
    .get();

```