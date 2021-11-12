---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 70f19ee804761fd060f0076adeb40569a4a981c463535a2888de315a78dabaf3
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57277451"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EndpointCollectionPage endpoints = graphClient.groups("{id}").endpoints()
    .buildRequest()
    .get();

```