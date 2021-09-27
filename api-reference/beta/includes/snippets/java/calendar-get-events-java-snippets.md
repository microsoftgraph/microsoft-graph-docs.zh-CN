---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 99e5fe27c3d98f2b6dea5e4e79012737d5df6e7466529c04200a2e4ba73877df
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57106187"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EventCollectionPage events = graphClient.me().calendar().events()
    .buildRequest()
    .get();

```